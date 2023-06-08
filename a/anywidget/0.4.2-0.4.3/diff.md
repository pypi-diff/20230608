# Comparing `tmp/anywidget-0.4.2.tar.gz` & `tmp/anywidget-0.4.3.tar.gz`

## Comparing `anywidget-0.4.2.tar` & `anywidget-0.4.3.tar`

### file list

```diff
@@ -1,102 +1,103 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.4.2/package.json
--rw-r--r--   0        0        0   259862 2020-02-02 00:00:00.000000 anywidget-0.4.2/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.2/pnpm-workspace.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.2/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/__init__.py
--rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/widget.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/138.60ddf4a50d830c18a721.js
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/326.53aec23a9e055d4c6252.js
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/remoteEntry.9229e22154b84f74e1ee.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.2/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/astro.config.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/scripts/render.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.2/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.2/examples/Counter.ipynb
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.4.2/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/package.json
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.2/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_descriptor.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_utils.py
--rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.2/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.2/LICENSE
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 anywidget-0.4.2/README.md
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 anywidget-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.4.3/CITATION.cff
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 anywidget-0.4.3/package.json
+-rw-r--r--   0        0        0   259862 2020-02-02 00:00:00.000000 anywidget-0.4.3/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.4.3/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.4.3/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/__init__.py
+-rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_util.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/widget.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/138.0afe77da678bd56cb574.js
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/326.34a64ac7689c2caccba1.js
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/remoteEntry.9d280f9a4b339dfca42d.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 anywidget-0.4.3/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5757 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.4.3/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 anywidget-0.4.3/examples/Counter.ipynb
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 anywidget-0.4.3/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     6121 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/package.json
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     5734 2020-02-02 00:00:00.000000 anywidget-0.4.3/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_descriptor.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_utils.py
+-rw-r--r--   0        0        0     5180 2020-02-02 00:00:00.000000 anywidget-0.4.3/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.4.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.4.3/LICENSE
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 anywidget-0.4.3/README.md
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 anywidget-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 anywidget-0.4.3/PKG-INFO
```

### Comparing `anywidget-0.4.2/.pre-commit-config.yaml` & `anywidget-0.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/package.json` & `anywidget-0.4.3/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/pnpm-lock.yaml` & `anywidget-0.4.3/pnpm-lock.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/anywidget/_descriptor.py` & `anywidget-0.4.3/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/anywidget/_file_contents.py` & `anywidget-0.4.3/anywidget/_file_contents.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,9 +85,9 @@
                     self._contents = None
                     self.changed.emit(str(self))
                     yield (change, path)
                     break
 
     def __str__(self) -> str:
         if self._contents is None:
-            self._contents = self._path.read_text()
+            self._contents = self._path.read_text(encoding="utf-8")
         return self._contents
```

### Comparing `anywidget-0.4.2/anywidget/_protocols.py` & `anywidget-0.4.3/anywidget/_protocols.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/anywidget/_util.py` & `anywidget-0.4.3/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/anywidget/experimental.py` & `anywidget-0.4.3/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/anywidget/widget.py` & `anywidget-0.4.3/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/anywidget/labextension/package.json` & `anywidget-0.4.3/anywidget/labextension/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95703125%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9d280f9a4b339dfca42d.js'}}",*

 * * "'version'": "'0.4.3'"}*

```diff
@@ -22,15 +22,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9229e22154b84f74e1ee.js"
+            "load": "static/remoteEntry.9d280f9a4b339dfca42d.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -42,9 +42,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.4.2"
+    "version": "0.4.3"
 }
```

### Comparing `anywidget-0.4.2/anywidget/labextension/static/138.60ddf4a50d830c18a721.js` & `anywidget-0.4.3/anywidget/labextension/static/138.0afe77da678bd56cb574.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -92,11 +92,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.2"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.3"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.2/anywidget/labextension/static/326.53aec23a9e055d4c6252.js` & `anywidget-0.4.3/anywidget/labextension/static/326.34a64ac7689c2caccba1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -110,11 +110,11 @@
                 return {
                     AnyModel: t,
                     AnyView: i
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.2"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.4.3"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.4.2/anywidget/labextension/static/remoteEntry.9229e22154b84f74e1ee.js` & `anywidget-0.4.3/anywidget/labextension/static/remoteEntry.9d280f9a4b339dfca42d.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, s, f, d, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, d, s, f, c, p, h, v = {
             408: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(138).then((() => () => t(138))),
                         "./extension": () => t.e(326).then((() => () => t(326)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -41,49 +41,49 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "60ddf4a50d830c18a721",
-        326: "53aec23a9e055d4c6252"
+        138: "0afe77da678bd56cb574",
+        326: "34a64ac7689c2caccba1"
     } [e] + ".js?v=" + {
-        138: "60ddf4a50d830c18a721",
-        326: "53aec23a9e055d4c6252"
+        138: "0afe77da678bd56cb574",
+        326: "34a64ac7689c2caccba1"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "anywidget:", m.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
-                for (var l = document.getElementsByTagName("script"), s = 0; s < l.length; s++) {
-                    var f = l[s];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
-                        i = f;
+                for (var l = document.getElementsByTagName("script"), d = 0; d < l.length; d++) {
+                    var s = l[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, m.nc && i.setAttribute("nonce", m.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(c);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -104,15 +104,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.4.2"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.4.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -161,80 +161,80 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var s, f, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(s = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
-                if ("u" == f) {
-                    if (!l || "u" != d) return !1
+                var d, s, f = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !l || ("u" == f ? u > n && !o : "" == f != o);
+                if ("u" == s) {
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (d == f)
+                    if (f == s)
                         if (u <= n) {
-                            if (s != e[u]) return !1
+                            if (d != e[u]) return !1
                         } else {
-                            if (o ? s > e[u] : s < e[u]) return !1;
-                            s != e[u] && (l = !1)
+                            if (o ? d > e[u] : d < e[u]) return !1;
+                            d != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != f && "n" != f) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || f < d != o) return !1;
+                    if (u <= n || s < f != o) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != f && "n" != f && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var c = [],
+            p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = m.S[e];
         if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+    }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", d = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), f(e[t][o])
-    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+        return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(e, t, o, n)), s(e[t][o])
+    }, s = e => (e.loaded = 1, e.get()), f = (e => function(r, t, n, o) {
         var a = m.I(r);
         return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), p = {}, c = {
-        395: () => d("default", "@jupyter-widgets/base", [, [1, 6],
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), c = {}, p = {
+        395: () => f("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2], 1, 1, 1, 1
         ])
     }, h = {
         326: [395]
     }, m.f.consumes = (e, r) => {
         m.o(h, e) && h[e].forEach((e => {
-            if (m.o(p, e)) return r.push(p[e]);
+            if (m.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    p[e] = 0, m.m[e] = t => {
+                    c[e] = 0, m.m[e] = t => {
                         delete m.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], m.m[e] = t => {
+                    delete c[e], m.m[e] = t => {
                         throw delete m.c[e], r
                     }
                 };
             try {
-                var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                var o = p[e]();
+                o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             957: 0
```

### Comparing `anywidget-0.4.2/anywidget/nbextension/index.js` & `anywidget-0.4.3/anywidget/nbextension/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.4.2";
+var version = "0.4.3";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
```

### Comparing `anywidget-0.4.2/docs/README.md` & `anywidget-0.4.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/astro.config.js` & `anywidget-0.4.3/docs/astro.config.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/package.json` & `anywidget-0.4.3/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/anywidget-overview.png` & `anywidget-0.4.3/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/banner-dark.png` & `anywidget-0.4.3/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/banner-light.png` & `anywidget-0.4.3/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/banner-minimal.png` & `anywidget-0.4.3/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/client-js-diagram.png` & `anywidget-0.4.3/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/default-og-image.png` & `anywidget-0.4.3/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/favicon.svg` & `anywidget-0.4.3/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/public/widget-overview.png` & `anywidget-0.4.3/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/scripts/ipynb.mjs` & `anywidget-0.4.3/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/scripts/utils.mjs` & `anywidget-0.4.3/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/consts.ts` & `anywidget-0.4.3/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/CodeHero.astro` & `anywidget-0.4.3/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/CounterButton.astro` & `anywidget-0.4.3/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/HeadCommon.astro` & `anywidget-0.4.3/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/HeadSEO.astro` & `anywidget-0.4.3/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Hero.astro` & `anywidget-0.4.3/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.4.3/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.4.3/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.4.3/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/Header.astro` & `anywidget-0.4.3/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/HeaderButton.css` & `anywidget-0.4.3/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.4.3/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.4.3/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/Search.css` & `anywidget-0.4.3/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/Search.tsx` & `anywidget-0.4.3/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.4.3/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.4.3/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.4.3/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.4.3/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.4.3/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.4.3/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.4.3/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/components/examples/Counter.astro` & `anywidget-0.4.3/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/layouts/MainLayout.astro` & `anywidget-0.4.3/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/layouts/SplashLayout.astro` & `anywidget-0.4.3/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.4.3/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.4.3/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/pages/en/bundling.md` & `anywidget-0.4.3/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/pages/en/experimental.md` & `anywidget-0.4.3/docs/src/pages/en/experimental.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/pages/en/getting-started.mdx` & `anywidget-0.4.3/docs/src/pages/en/getting-started.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.4.3/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.4.3/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/styles/index.css` & `anywidget-0.4.3/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/docs/src/styles/theme.css` & `anywidget-0.4.3/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/examples/Counter.ipynb` & `anywidget-0.4.3/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/examples/minimal_example.ipynb` & `anywidget-0.4.3/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/packages/anywidget/CHANGELOG.md` & `anywidget-0.4.3/packages/anywidget/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # anywidget
 
+## 0.4.3
+
+### Patch Changes
+
+- fix: Specify UTF-8 encoding in `FileContents.__str__` ([#135](https://github.com/manzt/anywidget/pull/135))
+
+  Fixes an `UnicodeDecodeError` observed on Windows when special characters are present in `_esm` or `_css` elements of a widget.
+
 ## 0.4.2
 
 ### Patch Changes
 
 - fix(descriptor): forward base obj repr for text/plain mimetype ([#131](https://github.com/manzt/anywidget/pull/131))
 
 ## 0.4.1
```

### Comparing `anywidget-0.4.2/packages/anywidget/build.mjs` & `anywidget-0.4.3/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/packages/anywidget/package.json` & `anywidget-0.4.3/packages/anywidget/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.4.3'"}*

```diff
@@ -38,9 +38,9 @@
     "name": "anywidget",
     "publishConfig": {
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs"
     },
-    "version": "0.4.2"
+    "version": "0.4.3"
 }
```

### Comparing `anywidget-0.4.2/packages/anywidget/src/widget.js` & `anywidget-0.4.3/packages/anywidget/src/widget.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/tests/test_descriptor.py` & `anywidget-0.4.3/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/tests/test_experimental.py` & `anywidget-0.4.3/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/tests/test_file_contents.py` & `anywidget-0.4.3/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/tests/test_utils.py` & `anywidget-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/tests/test_widget.py` & `anywidget-0.4.3/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/LICENSE` & `anywidget-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/README.md` & `anywidget-0.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # anywidget <a href="https://github.com/manzt/anywidget"><img align="right" src="https://raw.githubusercontent.com/manzt/anywidget/main/docs/public/favicon.svg" height="38"></img></a>
 
 [![PyPI](https://img.shields.io/pypi/v/anywidget.svg?color=green)](https://pypi.org/project/anywidget)
 [![License](https://img.shields.io/pypi/l/anywidget.svg?color=green)](https://github.com/manzt/anywidget/raw/main/LICENSE)
 [![codecov](https://codecov.io/gh/manzt/anywidget/branch/main/graph/badge.svg)](https://codecov.io/gh/manzt/anywidget)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/manzt/anywidget/blob/main/examples/Counter.ipynb)
+[![DOI](https://zenodo.org/badge/557583774.svg)](https://zenodo.org/badge/latestdoi/557583774)
 
 custom jupyter widgets made easy
 
 - 🛠️ create widgets **without complicated cookiecutter templates**
 - 📚 **publish to PyPI** like any other Python package
 - 🤖 prototype **within** `.ipynb` or `.py` files
 - 🚀 run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
```

### Comparing `anywidget-0.4.2/pyproject.toml` & `anywidget-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anywidget-0.4.2/PKG-INFO` & `anywidget-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.4.2
+Version: 0.4.3
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
 Requires-Python: >=3.7
 Requires-Dist: importlib-metadata; python_version < '3.8'
@@ -25,14 +25,15 @@
 
 # anywidget <a href="https://github.com/manzt/anywidget"><img align="right" src="https://raw.githubusercontent.com/manzt/anywidget/main/docs/public/favicon.svg" height="38"></img></a>
 
 [![PyPI](https://img.shields.io/pypi/v/anywidget.svg?color=green)](https://pypi.org/project/anywidget)
 [![License](https://img.shields.io/pypi/l/anywidget.svg?color=green)](https://github.com/manzt/anywidget/raw/main/LICENSE)
 [![codecov](https://codecov.io/gh/manzt/anywidget/branch/main/graph/badge.svg)](https://codecov.io/gh/manzt/anywidget)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/manzt/anywidget/blob/main/examples/Counter.ipynb)
+[![DOI](https://zenodo.org/badge/557583774.svg)](https://zenodo.org/badge/latestdoi/557583774)
 
 custom jupyter widgets made easy
 
 - 🛠️ create widgets **without complicated cookiecutter templates**
 - 📚 **publish to PyPI** like any other Python package
 - 🤖 prototype **within** `.ipynb` or `.py` files
 - 🚀 run in **Jupyter**, **JupyterLab**, **Google Colab**, **VSCode**, and more
```

