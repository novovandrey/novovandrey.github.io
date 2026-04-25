---
title: "Java Garbage Collector: Interview Notes"
date: 2026-04-25
tags: [java, jvm, garbage-collector, interview]
description: "A practical summary of Java Garbage Collection for senior backend interviews."
---

Garbage Collection is one of the key JVM mechanisms responsible for automatic memory management.  
In Java, developers do not explicitly free objects from heap memory. Instead, the JVM detects objects that are no longer reachable and reclaims their memory.

### What problem does GC solve?

GC solves the problem of reclaiming heap memory occupied by objects that are no longer used by the application.

A Java object can be collected when it is no longer reachable from GC roots.

Typical GC roots include:

- local variables in active stack frames
- static fields
- active threads
- JNI references
- internal JVM references

### Basic GC lifecycle

A simplified GC cycle usually consists of several phases:

1. **Mark**  
   The collector finds all objects that are still reachable.

2. **Sweep**  
   The collector identifies memory occupied by unreachable objects.

3. **Compact or relocate**  
   Some collectors move live objects to reduce fragmentation.

Not every garbage collector performs all phases in the same way.

### Generational hypothesis

Most Java applications create many short-lived objects.

Because of that, the heap is usually divided into generations:

- **Young Generation**  
  Stores newly created objects.

- **Old Generation**  
  Stores objects that survived multiple young collections.

Young GC is usually frequent and relatively cheap.  
Old GC is less frequent but usually more expensive.

### G1 GC

G1 splits the heap into multiple regions instead of using one continuous young and old space.

Its main idea is to collect regions with the most reclaimable memory first.

Important points:

- designed for large heaps
- predictable pause-time goal
- compacts memory by evacuating live objects between regions
- default GC in many modern Java versions

### ZGC

ZGC is a low-latency garbage collector.

Its main goal is to keep pause times very small, even with large heaps.

Important points:

- performs most work concurrently with application threads
- supports very large heaps
- uses load barriers
- focuses on low latency rather than maximum throughput

### Shenandoah

Shenandoah is also a low-latency collector.

It reduces pause times by doing concurrent evacuation and compaction.

Important points:

- performs marking, evacuation and reference updates mostly concurrently
- aims to make pause time less dependent on heap size
- useful for latency-sensitive applications

### Practical interview answer

A good short answer:

> Garbage Collection is the JVM mechanism that automatically reclaims heap memory by identifying objects that are no longer reachable from GC roots. Modern collectors such as G1, ZGC and Shenandoah differ mainly in how much work they do concurrently, how they handle compaction and whether they optimize for throughput or low latency.

### Common interview mistakes

Avoid saying that GC simply deletes unused objects immediately.

More precise wording:

- GC collects unreachable objects, not just unused objects
- collection is not immediate
- different collectors have different pause-time and throughput trade-offs
- low-latency collectors reduce pauses but may have additional runtime overhead

### Practical rule

For most backend services, G1 is a strong default choice.

For latency-sensitive systems with strict pause-time requirements, ZGC or Shenandoah may be considered after measurement.
