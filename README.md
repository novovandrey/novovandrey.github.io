
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Andrey Novov — Senior Java Developer</title>
  <meta name="description" content="Senior Java Developer: Java 21, Spring, Kafka, Kubernetes, Caffeine, high‑load." />
  <meta property="og:title" content="Andrey Novov — Senior Java Developer" />
  <meta property="og:description" content="Java 21, Spring, Kafka, Kubernetes. Experience: high‑load, performance, caching." />
  <meta property="og:type" content="website" />
  <meta property="og:image" content="/og-image.png" />
  <link rel="icon" href="/favicon.ico" />
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
  <style>
    /* IntelliJ‑like light theme */
:root { --accent:#0b76d1; --border:#d0d7e2; --panel:#ffffff; --panel-alt:#f6f8fa; }
body { font-family: Inter, ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji"; }
a { color: var(--accent); text-underline-offset: 2px; }
a:hover { text-decoration: underline; }
.focus-ring:focus-visible { outline: 2px solid var(--accent); outline-offset: 2px; border-radius: 12px; }
    /* Code tooltip */
    .tooltip { position: relative; }
    .tooltip .tip { pointer-events: none; position: absolute; z-index: 50; min-width: 16rem; max-width: 28rem; left: 50%; transform: translateX(-50%) translateY(8px); opacity: 0; transition: opacity .15s ease, transform .15s ease; }
    .tooltip:hover .tip, .tooltip:focus-within .tip { opacity: 1; transform: translateX(-50%) translateY(0); }
    /* Javadoc‑style block */
    .javadoc { font-family: "JetBrains Mono", ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace; }
    .code-card { background: #f6f8fa; color: #1f2937; border: 1px solid #d0d7e2; }
    .code-card .ann { color: #945bb0; }
    .code-card .type { color: #0b76d1; }
    .code-card .ident { color: #2aa198; }
    .code-card .kw { color: #a626a4; }
    .code-card .cm { color: #6b778d; }
    /* Package tree connector */
    .tree:before { content: ""; position: absolute; left: 0.75rem; top: 0; bottom: 0; width: 2px; background: rgba(2,6,23,0.12); }
  </style>
  <script>
    // Optional: Copy code sample from tooltip
    function copyCode(id) {
      const el = document.getElementById(id);
      if (!el) return;
      navigator.clipboard.writeText(el.innerText);
      const btn = el.closest('.tip').querySelector('button');
      if (btn) { const label = btn.innerText; btn.innerText = 'Copied'; setTimeout(()=>btn.innerText=label, 1200); }
    }
  </script>
  <script type="application/ld+json">
  {
    "@context":"https://schema.org",
    "@type":"Person",
    "name":"Andrey Novov",
    "jobTitle":"Senior Java Developer",
    "url":"https://novovandrey.github.io/",
    "email":"mailto:novov.andrew@gmail.com",
    "sameAs":["https://github.com/novovandrey","https://www.linkedin.com/in/andrei-novov-841b99b1/"],
    "knowsAbout":["Java 21","Spring","Kafka","Kubernetes","Caffeine","Akka Streams"]
  }
  </script>
</head>
<body class="bg-white min-h-screen text-gray-900 selection:bg-blue-100">
  <main class="max-w-5xl mx-auto px-6 py-10">
    <!-- Header -->
    <header class="flex flex-col sm:flex-row sm:items-center sm:justify-between gap-4 mb-10">
      <div class="text-slate-900">
        <h1 class="text-4xl font-extrabold tracking-tight">Andrey Novov</h1>
        <p class="text-lg/7 opacity-95">Senior Java Developer · Lisbon</p>
        <p class="text-sm/6 opacity-90"><a class="underline" href="mailto:novov.andrew@gmail.com">novov.andrew@gmail.com</a></p>
      </div>
      <div class="flex flex-wrap gap-3">
        <a class="focus-ring px-4 py-2 rounded-2xl bg-black/80 text-white hover:bg-black" href="/cv.pdf">Download PDF</a>
        <a class="focus-ring px-4 py-2 rounded-2xl bg-white text-slate-900 border border-slate-300 hover:bg-slate-50" href="https://github.com/novovandrey">GitHub</a>
        <a class="focus-ring px-4 py-2 rounded-2xl bg-white text-slate-900 border border-slate-300 hover:bg-slate-50" href="https://www.linkedin.com/in/andrei-novov-841b99b1/">LinkedIn</a>
      </div>
    </header>

    <!-- Tech Icons Row (Java ecosystem) -->
    <section class="mb-10">
      <div class="flex items-center gap-6 text-slate-700">
        <!-- Java steaming cup (inline SVG) -->
        <svg aria-label="Java" class="h-8" viewBox="0 0 64 64" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M20 46c6 4 24 4 30 0" stroke="currentColor" stroke-width="2"/>
          <path d="M24 40c5 3 19 3 24 0" stroke="currentColor" stroke-width="2"/>
          <path d="M28 34c3 2 13 2 16 0" stroke="currentColor" stroke-width="2"/>
          <path d="M36 12c6 6-6 8 2 14" stroke="currentColor" stroke-width="2"/>
          <path d="M30 16c6 6-6 8 2 14" stroke="currentColor" stroke-width="2"/>
        </svg>
        <!-- Spring leaf -->
        <svg aria-label="Spring" class="h-7" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
          <circle cx="32" cy="32" r="28" fill="#4CAF50"/>
          <path d="M44 24c-8 0-16 6-20 14-2 4 2 8 6 6 8-4 14-12 14-20z" fill="currentColor"/>
        </svg>
        <!-- Kafka (nodes) -->
        <svg aria-label="Kafka" class="h-7" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
          <circle cx="20" cy="32" r="8" fill="currentColor"/>
          <circle cx="44" cy="20" r="6" fill="currentColor"/>
          <circle cx="44" cy="44" r="6" fill="currentColor"/>
          <circle cx="32" cy="8" r="5" fill="currentColor"/>
          <circle cx="32" cy="56" r="5" fill="currentColor"/>
          <line x1="28" y1="28" x2="38" y2="22" stroke="currentColor" stroke-width="3"/>
          <line x1="28" y1="36" x2="38" y2="42" stroke="currentColor" stroke-width="3"/>
          <line x1="23" y1="26" x2="32" y2="13" stroke="currentColor" stroke-width="3"/>
          <line x1="23" y1="38" x2="32" y2="51" stroke="currentColor" stroke-width="3"/>
        </svg>
        <!-- JavaFX (stylized FX) -->
        <svg aria-label="JavaFX" class="h-7" viewBox="0 0 64 64" xmlns="http://www.w3.org/2000/svg">
          <rect x="6" y="10" width="52" height="44" rx="8" fill="none" stroke="currentColor" stroke-width="2"/>
          <text x="18" y="40" font-size="24" font-family="Verdana, Geneva, Tahoma, sans-serif" fill="#111">FX</text>
        </svg>
      </div>
    </section>

    <!-- About -->
    <section class="mb-12 bg-white border border-slate-200 rounded-2xl p-6 shadow-sm">
      <h2 class="text-xl font-semibold mb-2">About</h2>
      <p>Senior Java Developer with experience in high‑load systems: Java 21, Spring, Kafka, Kubernetes, Caffeine. Focus on latency optimization, cache design, and reliable integrations (IBM MQ, REST).</p>
    </section>

    <!-- Skills with interactive tooltips showing code samples -->
    <section class="mb-12 bg-white border border-slate-200 rounded-2xl p-6 shadow-sm">
      <h2 class="text-xl font-semibold mb-4">Skills</h2>
      <ul class="grid sm:grid-cols-2 lg:grid-cols-3 gap-4">
        <li class="tooltip">
          <button class="focus-ring w-full text-left px-4 py-3 rounded-xl border hover:border-black/40">Java 21 · Records/Concurrency</button>
          <div class="tip bg-slate-900 text-slate-100 rounded-xl p-4 shadow-xl border border-slate-700 mt-2">
            <div class="flex items-center justify-between gap-4 mb-2">
              <span class="text-sm opacity-80">Example: virtual threads</span>
              <button class="focus-ring text-xs px-2 py-1 rounded bg-slate-700" onclick="copyCode('code-java-virtual')">Copy</button>
            </div>
            <pre id="code-java-virtual" class="javadoc text-xs whitespace-pre-wrap">try (var scope = java.util.concurrent.StructuredTaskScope.ShutdownOnFailure.of()) {
  var r1 = scope.fork(() -> serviceA.call());
  var r2 = scope.fork(() -> serviceB.call());
  scope.join();
  return r1.result() + r2.result();
}</pre>
          </div>
        </li>
        <li class="tooltip">
          <button class="focus-ring w-full text-left px-4 py-3 rounded-xl border hover:border-black/40">Spring Boot · Observability</button>
          <div class="tip bg-slate-900 text-slate-100 rounded-xl p-4 shadow-xl border border-slate-700 mt-2">
            <div class="flex items-center justify-between gap-4 mb-2">
              <span class="text-sm opacity-80">Example: Micrometer + p95</span>
              <button class="focus-ring text-xs px-2 py-1 rounded bg-slate-700" onclick="copyCode('code-spring-metrics')">Copy</button>
            </div>
            <pre id="code-spring-metrics" class="javadoc text-xs whitespace-pre-wrap">@Timed(value = "checkout.latency", percentile = {0.5, 0.95})
public ResponseEntity&lt;Order&gt; checkout(...) { /* ... */ }</pre>
          </div>
        </li>
        <li class="tooltip">
          <button class="focus-ring w-full text-left px-4 py-3 rounded-xl border hover:border-black/40">Kafka · Exactly‑once / Retry</button>
          <div class="tip bg-slate-900 text-slate-100 rounded-xl p-4 shadow-xl border border-slate-700 mt-2">
            <div class="flex items-center justify-between gap-4 mb-2">
              <span class="text-sm opacity-80">Example: producer idempotence</span>
              <button class="focus-ring text-xs px-2 py-1 rounded bg-slate-700" onclick="copyCode('code-kafka-ido')">Copy</button>
            </div>
            <pre id="code-kafka-ido" class="javadoc text-xs whitespace-pre-wrap">props.put("enable.idempotence", true);
props.put("acks", "all");
props.put("max.in.flight.requests.per.connection", 1);</pre>
          </div>
        </li>
        <li class="tooltip">
          <button class="focus-ring w-full text-left px-4 py-3 rounded-xl border hover:border-black/40">Caffeine Cache · Tuning</button>
          <div class="tip bg-slate-900 text-slate-100 rounded-xl p-4 shadow-xl border border-slate-700 mt-2">
            <div class="flex items-center justify-between gap-4 mb-2">
              <span class="text-sm opacity-80">Example: p95‑latency drop</span>
              <button class="focus-ring text-xs px-2 py-1 rounded bg-slate-700" onclick="copyCode('code-caffeine')">Copy</button>
            </div>
            <pre id="code-caffeine" class="javadoc text-xs whitespace-pre-wrap">Cache&lt;Key, Val&gt; cache = Caffeine.newBuilder()
  .maximumSize(100_000)
  .recordStats()
  .expireAfterWrite(Duration.ofMinutes(5))
  .build(loader);
var stats = cache.stats(); // hitRate, evictionCount, etc.</pre>
          </div>
        </li>
        <li class="tooltip">
          <button class="focus-ring w-full text-left px-4 py-3 rounded-xl border hover:border-black/40">Kubernetes · GitOps</button>
          <div class="tip bg-slate-900 text-slate-100 rounded-xl p-4 shadow-xl border border-slate-700 mt-2">
            <div class="flex items-center justify-between gap-4 mb-2">
              <span class="text-sm opacity-80">Example: liveness/startup</span>
              <button class="focus-ring text-xs px-2 py-1 rounded bg-slate-700" onclick="copyCode('code-k8s')">Copy</button>
            </div>
            <pre id="code-k8s" class="javadoc text-xs whitespace-pre-wrap">livenessProbe:
  httpGet: { path: /actuator/health/liveness, port: 8080 }
startupProbe:
  httpGet: { path: /actuator/health/startup, port: 8080 }
  failureThreshold: 30
  periodSeconds: 10</pre>
          </div>
        </li>
      </ul>
    </section>

    <!-- Experience as Javadoc -->
    <section class="mb-12">
      <h2 class="text-xl font-semibold text-slate-900 mb-4">Experience</h2>
      <div class="grid gap-4">
        <article class="code-card rounded-2xl p-5">
          <pre class="javadoc text-sm whitespace-pre-wrap"><span class="cm">/**</span>
<span class="ann"> * @Description</span>  High‑load API optimization (‑35% p95 latency)
<span class="ann"> * @Role</span>         Senior Java Developer
<span class="ann"> * @Stack</span>        Java 21, Spring, Kafka, Caffeine, Kubernetes
<span class="cm"> */</span>
<span class="kw">public class</span> <span class="type">BNP Paribas Lisbon</span> <span class="kw">implements</span> <span class="type">BNP Paribas LLC</span> {
  <span class="kw">private</span> <span class="type">Cache</span>&lt;<span class="type">Key</span>, <span class="type">Val</span>&gt; <span class="ident">hotCache</span>;
  <span class="kw">public</span> <span class="type">Result</span> <span class="ident">process</span>(<span class="type">Request</span> req) { <span class="cm">/* ... */</span> }
}
</pre>
        </article>
        <article class="code-card rounded-2xl p-5">
          <pre class="javadoc text-sm whitespace-pre-wrap"><span class="cm">/**</span>
<span class="ann"> * @Description</span>  IBM MQ + REST integrations with two SSL contexts
<span class="ann"> * @Role</span>         Senior Java Developer
<span class="ann"> * @Stack</span>        Spring, IBM MQ, TLS, Observability
<span class="cm"> */</span>
<span class="kw">public class</span> <span class="type"></span> {
  <span class="kw">public class</span> <span class="type">T-Systems</span> <span class="kw">implements</span> <span class="type">Deutch Telekom</span> {
  <span class="type">SSLContext</span> <span class="ident">restCtx</span>, <span class="ident">mqCtx</span>;
  <span class="kw">void</span> <span class="ident">transfer</span>() { <span class="cm">/* retry, DLQ, alerts */</span> }
}
</pre>
        </article>
      </div>
    </section>

    <!-- Projects as package/class tree -->
    <section class="mb-12 bg-white border border-slate-200 rounded-2xl p-6 shadow-sm relative">
      <h2 class="text-xl font-semibold mb-4">Projects</h2>
      <ul class="space-y-4 pl-6 relative tree">
        <li>
          <div class="font-mono text-sm">dev.novov.projects.<span class="font-semibold">RehypoViewer</span></div>
          <div class="mt-1 text-sm text-gray-700">Class: <span class="font-mono">RehypoViewer</span> — web app for data visualization; <span class="font-mono">public void optimize()</span> reduces rendering overhead.</div>
          <div class="mt-2"><a class="underline" href="#">Source</a> · <a class="underline" href="#">Demo</a></div>
        </li>
        <li>
          <div class="font-mono text-sm">dev.novov.projects.<span class="font-semibold">KafkaPipelines</span></div>
          <div class="mt-1 text-sm text-gray-700">Class: <span class="font-mono">RetryOrchestrator</span> — retries with backoff, DLQ, exactly‑once semantics.</div>
        </li>
        <li>
          <div class="font-mono text-sm">dev.novov.projects.<span class="font-semibold">CacheInspector</span></div>
          <div class="mt-1 text-sm text-gray-700">Class: <span class="font-mono">CaffeineStats</span> — metrics, hitRate, evictionCount, Prometheus export.</div>
        </li>
      </ul>
    </section>

    <footer class="text-slate-600 text-sm">© Andrey Novov — Java ecosystem, 2025</footer>
  </main>
</body>
</html>
