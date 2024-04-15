# Comparing `tmp/gradio_highlightedtextbox-0.0.8.tar.gz` & `tmp/gradio_highlightedtextbox-0.0.9.tar.gz`

## Comparing `gradio_highlightedtextbox-0.0.8.tar` & `gradio_highlightedtextbox-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/__init__.py
--rw-r--r--   0        0        0    13040 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/highlightedtextbox.py
--rw-r--r--   0        0        0    43709 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/highlightedtextbox.pyi
--rw-r--r--   0        0        0    75550 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/templates/component/index.js
--rw-r--r--   0        0        0    15020 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/templates/component/style.css
--rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/templates/example/index.js
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/templates/example/style.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/demo/__init__.py
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/demo/app.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/demo/css.css
--rw-r--r--   0        0        0    13932 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/demo/space.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/frontend/BlockTitleWithHighlights.svelte
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/frontend/Example.svelte
--rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/frontend/HighlightedTextbox.svelte
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/frontend/Index.svelte
--rw-r--r--   0        0        0    33510 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/frontend/package-lock.json
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/frontend/package.json
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/frontend/utils.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/.gitignore
--rw-r--r--   0        0        0    13244 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/README.md
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    14459 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/__init__.py
+-rw-r--r--   0        0        0    13270 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/highlightedtextbox.py
+-rw-r--r--   0        0        0    49044 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/highlightedtextbox.pyi
+-rw-r--r--   0        0        0    81968 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/templates/component/index.js
+-rw-r--r--   0        0        0    15422 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/templates/component/style.css
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/templates/example/index.js
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/templates/example/style.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/demo/__init__.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/demo/app.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/demo/css.css
+-rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/demo/space.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/BlockTitleWithHighlights.svelte
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/Copy.svelte
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/Example.svelte
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/HighlightedTextbox.svelte
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/Index.svelte
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/RemoveTags.svelte
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/Widgets.svelte
+-rw-r--r--   0        0        0    33510 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/package-lock.json
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/package.json
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/frontend/utils.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/.gitignore
+-rw-r--r--   0        0        0    13695 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    14910 2020-02-02 00:00:00.000000 gradio_highlightedtextbox-0.0.9/PKG-INFO
```

### Comparing `gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/highlightedtextbox.py` & `gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/highlightedtextbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     EVENTS = [
         Events.change,
         Events.input,
         Events.select,
         Events.submit,
         Events.focus,
         Events.blur,
+        Events.clear,
     ]
     data_model = HighlightedTextData
 
     def __init__(
         self,
         value: list[tuple[str, str | None]] | Callable | None = "",
         *,
@@ -57,14 +58,15 @@
         elem_id: str | None = None,
         autofocus: bool = False,
         autoscroll: bool = True,
         interactive: bool = True,
         elem_classes: list[str] | str | None = None,
         render: bool = True,
         show_copy_button: bool = False,
+        show_remove_tags_button: bool = False,
     ):
         """
         Parameters:
             value: default text to provide in textbox. If callable, the function will be called whenever the app loads to set the initial value of the component.
             lines: number of lines to display in textbox.
             max_lines: maximum number of lines to display in textbox.
             color_map: dictionary mapping labels to colors.
@@ -85,24 +87,26 @@
             rtl: If True and `type` is "text", sets the direction of the text to right-to-left (cursor appears on the left of the text). Default is False, which renders cursor on the right.
             elem_id: An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.
             elem_classes: An optional list of strings that are assigned as the classes of this component in the HTML DOM. Can be used for targeting CSS styles.
             render: If False, component will not render be rendered in the Blocks context. Should be used if the intention is to assign event listeners now but render the component later.
             rtl: If True and `type` is "text", sets the direction of the text to right-to-left (cursor appears on the left of the text). Default is False, which renders cursor on the right.
             show_copy_button: If True, includes a copy button to copy the text in the textbox. Only applies if show_label is True.
             autoscroll: If True, will automatically scroll to the bottom of the textbox when the value changes, unless the user scrolls up. If False, will not scroll to the bottom of the textbox when the value changes.
+            show_remove_tags_button: If True, includes a button to remove all tags from the text.
         """
         self.color_map = color_map
         self.show_legend = show_legend
         self.show_legend_label = show_legend_label
         self.legend_label = legend_label
         self.combine_adjacent = combine_adjacent
         self.adjacent_separator = adjacent_separator
         self.show_copy_button = show_copy_button
         self.autofocus = autofocus
         self.autoscroll = autoscroll
+        self.show_remove_tags_button = show_remove_tags_button
         super().__init__(
             label=label,
             info=info,
             show_label=show_label,
             container=container,
             scale=scale,
             min_width=min_width,
```

### Comparing `gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/highlightedtextbox.pyi` & `gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/highlightedtextbox.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     EVENTS = [
         Events.change,
         Events.input,
         Events.select,
         Events.submit,
         Events.focus,
         Events.blur,
+        Events.clear,
     ]
     data_model = HighlightedTextData
 
     def __init__(
         self,
         value: list[tuple[str, str | None]] | Callable | None = "",
         *,
@@ -58,14 +59,15 @@
         elem_id: str | None = None,
         autofocus: bool = False,
         autoscroll: bool = True,
         interactive: bool = True,
         elem_classes: list[str] | str | None = None,
         render: bool = True,
         show_copy_button: bool = False,
+        show_remove_tags_button: bool = False,
     ):
         """
         Parameters:
             value: default text to provide in textbox. If callable, the function will be called whenever the app loads to set the initial value of the component.
             lines: number of lines to display in textbox.
             max_lines: maximum number of lines to display in textbox.
             color_map: dictionary mapping labels to colors.
@@ -86,24 +88,26 @@
             rtl: If True and `type` is "text", sets the direction of the text to right-to-left (cursor appears on the left of the text). Default is False, which renders cursor on the right.
             elem_id: An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.
             elem_classes: An optional list of strings that are assigned as the classes of this component in the HTML DOM. Can be used for targeting CSS styles.
             render: If False, component will not render be rendered in the Blocks context. Should be used if the intention is to assign event listeners now but render the component later.
             rtl: If True and `type` is "text", sets the direction of the text to right-to-left (cursor appears on the left of the text). Default is False, which renders cursor on the right.
             show_copy_button: If True, includes a copy button to copy the text in the textbox. Only applies if show_label is True.
             autoscroll: If True, will automatically scroll to the bottom of the textbox when the value changes, unless the user scrolls up. If False, will not scroll to the bottom of the textbox when the value changes.
+            show_remove_tags_button: If True, includes a button to remove all tags from the text.
         """
         self.color_map = color_map
         self.show_legend = show_legend
         self.show_legend_label = show_legend_label
         self.legend_label = legend_label
         self.combine_adjacent = combine_adjacent
         self.adjacent_separator = adjacent_separator
         self.show_copy_button = show_copy_button
         self.autofocus = autofocus
         self.autoscroll = autoscroll
+        self.show_remove_tags_button = show_remove_tags_button
         super().__init__(
             label=label,
             info=info,
             show_label=show_label,
             container=container,
             scale=scale,
             min_width=min_width,
@@ -498,14 +502,56 @@
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
         api_name: str | None | Literal[False] = None,
         scroll_to_output: bool = False,
         show_progress: Literal["full", "minimal", "hidden"] = "full",
         queue: bool | None = None,
+        batch: bool = False,
+        max_batch_size: int = 4,
+        preprocess: bool = True,
+        postprocess: bool = True,
+        cancels: dict[str, Any] | list[dict[str, Any]] | None = None,
+        every: float | None = None,
+        trigger_mode: Literal["once", "multiple", "always_last"] | None = None,
+        js: str | None = None,
+        concurrency_limit: int | None | Literal["default"] = "default",
+        concurrency_id: str | None = None,
+        show_api: bool = True) -> Dependency:
+        """
+        Parameters:
+            fn: the function to call when this event is triggered. Often a machine learning model's prediction function. Each parameter of the function corresponds to one input component, and the function should return a single value or a tuple of values, with each element in the tuple corresponding to one output component.
+            inputs: List of gradio.components to use as inputs. If the function takes no inputs, this should be an empty list.
+            outputs: List of gradio.components to use as outputs. If the function returns no outputs, this should be an empty list.
+            api_name: Defines how the endpoint appears in the API docs. Can be a string, None, or False. If False, the endpoint will not be exposed in the api docs. If set to None, the endpoint will be exposed in the api docs as an unnamed endpoint, although this behavior will be changed in Gradio 4.0. If set to a string, the endpoint will be exposed in the api docs with the given name.
+            scroll_to_output: If True, will scroll to output component on completion
+            show_progress: If True, will show progress animation while pending
+            queue: If True, will place the request on the queue, if the queue has been enabled. If False, will not put this event on the queue, even if the queue has been enabled. If None, will use the queue setting of the gradio app.
+            batch: If True, then the function should process a batch of inputs, meaning that it should accept a list of input values for each parameter. The lists should be of equal length (and be up to length `max_batch_size`). The function is then *required* to return a tuple of lists (even if there is only 1 output component), with each list in the tuple corresponding to one output component.
+            max_batch_size: Maximum number of inputs to batch together if this is called from the queue (only relevant if batch=True)
+            preprocess: If False, will not run preprocessing of component data before running 'fn' (e.g. leaving it as a base64 string if this method is called with the `Image` component).
+            postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
+            cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
+            every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds. Queue must be enabled.
+            trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` event) would allow a second submission after the pending event is complete.
+            js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
+            concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
+            concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
+        """
+        ...
+    
+    def clear(self,
+        fn: Callable | None,
+        inputs: Component | Sequence[Component] | set[Component] | None = None,
+        outputs: Component | Sequence[Component] | None = None,
+        api_name: str | None | Literal[False] = None,
+        scroll_to_output: bool = False,
+        show_progress: Literal["full", "minimal", "hidden"] = "full",
+        queue: bool | None = None,
         batch: bool = False,
         max_batch_size: int = 4,
         preprocess: bool = True,
         postprocess: bool = True,
         cancels: dict[str, Any] | list[dict[str, Any]] | None = None,
         every: float | None = None,
         trigger_mode: Literal["once", "multiple", "always_last"] | None = None,
```

### Comparing `gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/templates/component/index.js` & `gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/templates/component/index.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,52 +1,52 @@
 const {
-    SvelteComponent: ll,
-    append: oe,
+    SvelteComponent: yl,
+    append: se,
     attr: U,
-    create_slot: nl,
-    destroy_each: il,
+    create_slot: Cl,
+    destroy_each: ql,
     detach: fe,
-    element: ue,
-    empty: sl,
+    element: de,
+    empty: Tl,
     ensure_array_like: tt,
-    get_all_dirty_from_scope: ol,
-    get_slot_changes: fl,
-    init: _l,
+    get_all_dirty_from_scope: Sl,
+    get_slot_changes: Ll,
+    init: jl,
     insert: _e,
-    safe_not_equal: al,
-    set_data: Xe,
-    space: He,
-    text: Ye,
+    safe_not_equal: Fl,
+    set_data: Je,
+    space: Me,
+    text: Ke,
     toggle_class: V,
-    transition_in: rl,
-    transition_out: ul,
-    update_slot_base: cl
+    transition_in: Hl,
+    transition_out: Ml,
+    update_slot_base: Nl
 } = window.__gradio__svelte__internal;
 
 function lt(l, e, t) {
     const n = l.slice();
     return n[8] = e[t][0], n[9] = e[t][1], n[11] = t, n;
 }
 
 function nt(l) {
-    let e, t, n, i, s, o, r = tt(Object.entries(
+    let e, t, n, i, o, s, f = tt(Object.entries(
             /*_color_map*/
             l[4]
         )),
         a = [];
-    for (let f = 0; f < r.length; f += 1)
-        a[f] = it(lt(l, r, f));
+    for (let _ = 0; _ < f.length; _ += 1)
+        a[_] = it(lt(l, f, _));
     return {
         c() {
-            e = ue("span"), e.textContent = "·", t = He(), n = ue("div"), i = ue("span"), s = Ye(
+            e = de("span"), e.textContent = "·", t = Me(), n = de("div"), i = de("span"), o = Ke(
                 /*legend_label*/
                 l[3]
-            ), o = He();
-            for (let f = 0; f < a.length; f += 1)
-                a[f].c();
+            ), s = Me();
+            for (let _ = 0; _ < a.length; _ += 1)
+                a[_].c();
             U(e, "class", "legend-separator svelte-vm3q5z"), V(e, "hide", ! /*show_legend*/
                 l[1] || ! /*show_label*/
                 l[0]), V(
                 e,
                 "has-info",
                 /*info*/
                 l[5] != null
@@ -55,492 +55,822 @@
                 i,
                 "has-info",
                 /*info*/
                 l[5] != null
             ), U(n, "class", "category-legend svelte-vm3q5z"), U(n, "data-testid", "highlighted-text:category-legend"), V(n, "hide", ! /*show_legend*/
                 l[1]);
         },
-        m(f, _) {
-            _e(f, e, _), _e(f, t, _), _e(f, n, _), oe(n, i), oe(i, s), oe(n, o);
+        m(_, r) {
+            _e(_, e, r), _e(_, t, r), _e(_, n, r), se(n, i), se(i, o), se(n, s);
             for (let u = 0; u < a.length; u += 1)
                 a[u] && a[u].m(n, null);
         },
-        p(f, _) {
-            if (_ & /*show_legend, show_label*/
+        p(_, r) {
+            if (r & /*show_legend, show_label*/
                 3 && V(e, "hide", ! /*show_legend*/
-                    f[1] || ! /*show_label*/
-                    f[0]), _ & /*info*/
+                    _[1] || ! /*show_label*/
+                    _[0]), r & /*info*/
                 32 && V(
                     e,
                     "has-info",
                     /*info*/
-                    f[5] != null
-                ), _ & /*legend_label*/
-                8 && Xe(
-                    s,
+                    _[5] != null
+                ), r & /*legend_label*/
+                8 && Je(
+                    o,
                     /*legend_label*/
-                    f[3]
-                ), _ & /*show_legend_label*/
+                    _[3]
+                ), r & /*show_legend_label*/
                 4 && V(i, "hide", ! /*show_legend_label*/
-                    f[2]), _ & /*info*/
+                    _[2]), r & /*info*/
                 32 && V(
                     i,
                     "has-info",
                     /*info*/
-                    f[5] != null
-                ), _ & /*Object, _color_map, info*/
+                    _[5] != null
+                ), r & /*Object, _color_map, info*/
                 48) {
-                r = tt(Object.entries(
+                f = tt(Object.entries(
                     /*_color_map*/
-                    f[4]
+                    _[4]
                 ));
                 let u;
-                for (u = 0; u < r.length; u += 1) {
-                    const c = lt(f, r, u);
-                    a[u] ? a[u].p(c, _) : (a[u] = it(c), a[u].c(), a[u].m(n, null));
+                for (u = 0; u < f.length; u += 1) {
+                    const c = lt(_, f, u);
+                    a[u] ? a[u].p(c, r) : (a[u] = it(c), a[u].c(), a[u].m(n, null));
                 }
                 for (; u < a.length; u += 1)
                     a[u].d(1);
-                a.length = r.length;
+                a.length = f.length;
             }
-            _ & /*show_legend*/
+            r & /*show_legend*/
                 2 && V(n, "hide", ! /*show_legend*/
-                    f[1]);
+                    _[1]);
         },
-        d(f) {
-            f && (fe(e), fe(t), fe(n)), il(a, f);
+        d(_) {
+            _ && (fe(e), fe(t), fe(n)), ql(a, _);
         }
     };
 }
 
 function it(l) {
     let e, t = (
             /*category*/
             l[8] + ""
         ),
-        n, i, s;
+        n, i, o;
     return {
         c() {
-            e = ue("div"), n = Ye(t), i = He(), U(e, "class", "category-label svelte-vm3q5z"), U(e, "style", s = "background-color:" + /*color*/
+            e = de("div"), n = Ke(t), i = Me(), U(e, "class", "category-label svelte-vm3q5z"), U(e, "style", o = "background-color:" + /*color*/
                 l[9].secondary), V(
                 e,
                 "has-info",
                 /*info*/
                 l[5] != null
             );
         },
-        m(o, r) {
-            _e(o, e, r), oe(e, n), oe(e, i);
+        m(s, f) {
+            _e(s, e, f), se(e, n), se(e, i);
         },
-        p(o, r) {
-            r & /*_color_map*/
+        p(s, f) {
+            f & /*_color_map*/
                 16 && t !== (t = /*category*/
-                    o[8] + "") && Xe(n, t), r & /*_color_map*/
-                16 && s !== (s = "background-color:" + /*color*/
-                    o[9].secondary) && U(e, "style", s), r & /*info*/
+                    s[8] + "") && Je(n, t), f & /*_color_map*/
+                16 && o !== (o = "background-color:" + /*color*/
+                    s[9].secondary) && U(e, "style", o), f & /*info*/
                 32 && V(
                     e,
                     "has-info",
                     /*info*/
-                    o[5] != null
+                    s[5] != null
                 );
         },
-        d(o) {
-            o && fe(e);
+        d(s) {
+            s && fe(e);
         }
     };
 }
 
-function st(l) {
+function ot(l) {
     let e, t;
     return {
         c() {
-            e = ue("div"), t = Ye(
+            e = de("div"), t = Ke(
                 /*info*/
                 l[5]
             ), U(e, "class", "title-with-highlights-info svelte-vm3q5z");
         },
         m(n, i) {
-            _e(n, e, i), oe(e, t);
+            _e(n, e, i), se(e, t);
         },
         p(n, i) {
             i & /*info*/
-                32 && Xe(
+                32 && Je(
                     t,
                     /*info*/
                     n[5]
                 );
         },
         d(n) {
             n && fe(e);
         }
     };
 }
 
-function dl(l) {
+function Vl(l) {
     let e, t, n, i = Object.keys(
             /*_color_map*/
             l[4]
         ).length !== 0,
-        s, o, r;
+        o, s, f;
     const a = (
             /*#slots*/
             l[7].default
         ),
-        f = nl(
+        _ = Cl(
             a,
             l,
             /*$$scope*/
             l[6],
             null
         );
-    let _ = i && nt(l),
+    let r = i && nt(l),
         u = (
             /*info*/
-            l[5] && st(l)
+            l[5] && ot(l)
         );
     return {
         c() {
-            e = ue("div"), t = ue("span"), f && f.c(), n = He(), _ && _.c(), s = He(), u && u.c(), o = sl(), U(t, "data-testid", "block-info"), U(t, "class", "svelte-vm3q5z"), V(t, "sr-only", ! /*show_label*/
+            e = de("div"), t = de("span"), _ && _.c(), n = Me(), r && r.c(), o = Me(), u && u.c(), s = Tl(), U(t, "data-testid", "block-info"), U(t, "class", "svelte-vm3q5z"), V(t, "sr-only", ! /*show_label*/
                 l[0]), V(t, "hide", ! /*show_label*/
                 l[0]), V(
                 t,
                 "has-info",
                 /*info*/
                 l[5] != null
             ), U(e, "class", "title-container svelte-vm3q5z");
         },
         m(c, m) {
-            _e(c, e, m), oe(e, t), f && f.m(t, null), oe(e, n), _ && _.m(e, null), _e(c, s, m), u && u.m(c, m), _e(c, o, m), r = !0;
+            _e(c, e, m), se(e, t), _ && _.m(t, null), se(e, n), r && r.m(e, null), _e(c, o, m), u && u.m(c, m), _e(c, s, m), f = !0;
         },
         p(c, [m]) {
-            f && f.p && (!r || m & /*$$scope*/
-                    64) && cl(
-                    f,
+            _ && _.p && (!f || m & /*$$scope*/
+                    64) && Nl(
+                    _,
                     a,
                     c,
                     /*$$scope*/
                     c[6],
-                    r ? fl(
+                    f ? Ll(
                         a,
                         /*$$scope*/
                         c[6],
                         m,
                         null
-                    ) : ol(
+                    ) : Sl(
                         /*$$scope*/
                         c[6]
                     ),
                     null
-                ), (!r || m & /*show_label*/
+                ), (!f || m & /*show_label*/
                     1) && V(t, "sr-only", ! /*show_label*/
-                    c[0]), (!r || m & /*show_label*/
+                    c[0]), (!f || m & /*show_label*/
                     1) && V(t, "hide", ! /*show_label*/
-                    c[0]), (!r || m & /*info*/
+                    c[0]), (!f || m & /*info*/
                     32) && V(
                     t,
                     "has-info",
                     /*info*/
                     c[5] != null
                 ), m & /*_color_map*/
                 16 && (i = Object.keys(
                     /*_color_map*/
                     c[4]
-                ).length !== 0), i ? _ ? _.p(c, m) : (_ = nt(c), _.c(), _.m(e, null)) : _ && (_.d(1), _ = null), /*info*/
-                c[5] ? u ? u.p(c, m) : (u = st(c), u.c(), u.m(o.parentNode, o)) : u && (u.d(1), u = null);
+                ).length !== 0), i ? r ? r.p(c, m) : (r = nt(c), r.c(), r.m(e, null)) : r && (r.d(1), r = null), /*info*/
+                c[5] ? u ? u.p(c, m) : (u = ot(c), u.c(), u.m(s.parentNode, s)) : u && (u.d(1), u = null);
         },
         i(c) {
-            r || (rl(f, c), r = !0);
+            f || (Hl(_, c), f = !0);
         },
         o(c) {
-            ul(f, c), r = !1;
+            Ml(_, c), f = !1;
         },
         d(c) {
-            c && (fe(e), fe(s), fe(o)), f && f.d(c), _ && _.d(), u && u.d(c);
+            c && (fe(e), fe(o), fe(s)), _ && _.d(c), r && r.d(), u && u.d(c);
         }
     };
 }
 
-function ml(l, e, t) {
+function zl(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: i
     } = e, {
-        show_label: s = !0
+        show_label: o = !0
     } = e, {
-        show_legend: o = !0
+        show_legend: s = !0
     } = e, {
-        show_legend_label: r = !0
+        show_legend_label: f = !0
     } = e, {
         legend_label: a = "Highlights:"
     } = e, {
-        _color_map: f = {}
+        _color_map: _ = {}
     } = e, {
-        info: _ = void 0
+        info: r = void 0
     } = e;
     return l.$$set = (u) => {
-        "show_label" in u && t(0, s = u.show_label), "show_legend" in u && t(1, o = u.show_legend), "show_legend_label" in u && t(2, r = u.show_legend_label), "legend_label" in u && t(3, a = u.legend_label), "_color_map" in u && t(4, f = u._color_map), "info" in u && t(5, _ = u.info), "$$scope" in u && t(6, i = u.$$scope);
+        "show_label" in u && t(0, o = u.show_label), "show_legend" in u && t(1, s = u.show_legend), "show_legend_label" in u && t(2, f = u.show_legend_label), "legend_label" in u && t(3, a = u.legend_label), "_color_map" in u && t(4, _ = u._color_map), "info" in u && t(5, r = u.info), "$$scope" in u && t(6, i = u.$$scope);
     }, [
-        s,
         o,
-        r,
-        a,
+        s,
         f,
+        a,
         _,
+        r,
         i,
         n
     ];
 }
-class hl extends ll {
+class El extends yl {
     constructor(e) {
-        super(), _l(this, e, ml, dl, al, {
+        super(), jl(this, e, zl, Vl, Fl, {
             show_label: 0,
             show_legend: 1,
             show_legend_label: 2,
             legend_label: 3,
             _color_map: 4,
             info: 5
         });
     }
 }
-const {
-    SvelteComponent: bl,
-    append: gl,
-    attr: le,
-    detach: wl,
-    init: kl,
-    insert: vl,
-    noop: Re,
-    safe_not_equal: pl,
-    svg_element: ot
-} = window.__gradio__svelte__internal;
 
-function yl(l) {
-    let e, t;
-    return {
-        c() {
-            e = ot("svg"), t = ot("polyline"), le(t, "points", "20 6 9 17 4 12"), le(e, "xmlns", "http://www.w3.org/2000/svg"), le(e, "viewBox", "2 0 20 20"), le(e, "fill", "none"), le(e, "stroke", "currentColor"), le(e, "stroke-width", "3"), le(e, "stroke-linecap", "round"), le(e, "stroke-linejoin", "round");
-        },
-        m(n, i) {
-            vl(n, e, i), gl(e, t);
-        },
-        p: Re,
-        i: Re,
-        o: Re,
-        d(n) {
-            n && wl(e);
-        }
-    };
-}
-class Cl extends bl {
-    constructor(e) {
-        super(), kl(this, e, null, yl, pl, {});
-    }
-}
-const {
-    SvelteComponent: ql,
-    append: ft,
-    attr: ae,
-    detach: Tl,
-    init: Ll,
-    insert: Sl,
-    noop: Ae,
-    safe_not_equal: Fl,
-    svg_element: De
-} = window.__gradio__svelte__internal;
-
-function Hl(l) {
-    let e, t, n;
-    return {
-        c() {
-            e = De("svg"), t = De("path"), n = De("path"), ae(t, "fill", "currentColor"), ae(t, "d", "M28 10v18H10V10h18m0-2H10a2 2 0 0 0-2 2v18a2 2 0 0 0 2 2h18a2 2 0 0 0 2-2V10a2 2 0 0 0-2-2Z"), ae(n, "fill", "currentColor"), ae(n, "d", "M4 18H2V4a2 2 0 0 1 2-2h14v2H4Z"), ae(e, "xmlns", "http://www.w3.org/2000/svg"), ae(e, "viewBox", "0 0 33 33"), ae(e, "color", "currentColor");
-        },
-        m(i, s) {
-            Sl(i, e, s), ft(e, t), ft(e, n);
-        },
-        p: Ae,
-        i: Ae,
-        o: Ae,
-        d(i) {
-            i && Tl(e);
-        }
-    };
-}
-class Ml extends ql {
-    constructor(e) {
-        super(), Ll(this, e, null, Hl, Fl, {});
-    }
-}
-
-function Ee() {}
-const jl = (l) => l;
+function Re() {}
+const Rl = (l) => l;
 
-function Nl(l, e) {
+function Dl(l, e) {
     return l != l ? e == e : l !== e || l && typeof l == "object" || typeof l == "function";
 }
-const It = typeof window < "u";
-let _t = It ? () => window.performance.now() : () => Date.now(),
-    Wt = It ? (l) => requestAnimationFrame(l) : Ee;
+const tl = typeof window < "u";
+let st = tl ? () => window.performance.now() : () => Date.now(),
+    ll = tl ? (l) => requestAnimationFrame(l) : Re;
 const Ce = /* @__PURE__ */ new Set();
 
-function Ut(l) {
+function nl(l) {
     Ce.forEach((e) => {
         e.c(l) || (Ce.delete(e), e.f());
-    }), Ce.size !== 0 && Wt(Ut);
+    }), Ce.size !== 0 && ll(nl);
 }
 
-function Vl(l) {
+function Bl(l) {
     let e;
-    return Ce.size === 0 && Wt(Ut), {
+    return Ce.size === 0 && ll(nl), {
         promise: new Promise((t) => {
             Ce.add(e = {
                 c: l,
                 f: t
             });
         }),
         abort() {
             Ce.delete(e);
         }
     };
 }
 
-function zl(l, {
+function ft(l, {
     delay: e = 0,
     duration: t = 400,
-    easing: n = jl
+    easing: n = Rl
 } = {}) {
     const i = +getComputedStyle(l).opacity;
     return {
         delay: e,
         duration: t,
         easing: n,
-        css: (s) => `opacity: ${s * i}`
+        css: (o) => `opacity: ${o * i}`
     };
 }
 const ve = [];
 
-function Bl(l, e = Ee) {
+function Pl(l, e = Re) {
     let t;
     const n = /* @__PURE__ */ new Set();
 
-    function i(r) {
-        if (Nl(l, r) && (l = r, t)) {
+    function i(f) {
+        if (Dl(l, f) && (l = f, t)) {
             const a = !ve.length;
-            for (const f of n)
-                f[1](), ve.push(f, l);
+            for (const _ of n)
+                _[1](), ve.push(_, l);
             if (a) {
-                for (let f = 0; f < ve.length; f += 2)
-                    ve[f][0](ve[f + 1]);
+                for (let _ = 0; _ < ve.length; _ += 2)
+                    ve[_][0](ve[_ + 1]);
                 ve.length = 0;
             }
         }
     }
 
-    function s(r) {
-        i(r(l));
+    function o(f) {
+        i(f(l));
     }
 
-    function o(r, a = Ee) {
-        const f = [r, a];
-        return n.add(f), n.size === 1 && (t = e(i, s) || Ee), r(l), () => {
-            n.delete(f), n.size === 0 && t && (t(), t = null);
+    function s(f, a = Re) {
+        const _ = [f, a];
+        return n.add(_), n.size === 1 && (t = e(i, o) || Re), f(l), () => {
+            n.delete(_), n.size === 0 && t && (t(), t = null);
         };
     }
     return {
         set: i,
-        update: s,
-        subscribe: o
+        update: o,
+        subscribe: s
     };
 }
 
-function at(l) {
+function _t(l) {
     return Object.prototype.toString.call(l) === "[object Date]";
 }
 
-function We(l, e, t, n) {
-    if (typeof t == "number" || at(t)) {
+function Ye(l, e, t, n) {
+    if (typeof t == "number" || _t(t)) {
         const i = n - t,
-            s = (t - e) / (l.dt || 1 / 60),
-            o = l.opts.stiffness * i,
-            r = l.opts.damping * s,
-            a = (o - r) * l.inv_mass,
-            f = (s + a) * l.dt;
-        return Math.abs(f) < l.opts.precision && Math.abs(i) < l.opts.precision ? n : (l.settled = !1, at(t) ? new Date(t.getTime() + f) : t + f);
+            o = (t - e) / (l.dt || 1 / 60),
+            s = l.opts.stiffness * i,
+            f = l.opts.damping * o,
+            a = (s - f) * l.inv_mass,
+            _ = (o + a) * l.dt;
+        return Math.abs(_) < l.opts.precision && Math.abs(i) < l.opts.precision ? n : (l.settled = !1, _t(t) ? new Date(t.getTime() + _) : t + _);
     } else {
         if (Array.isArray(t))
             return t.map(
-                (i, s) => We(l, e[s], t[s], n[s])
+                (i, o) => Ye(l, e[o], t[o], n[o])
             );
         if (typeof t == "object") {
             const i = {};
-            for (const s in t)
-                i[s] = We(l, e[s], t[s], n[s]);
+            for (const o in t)
+                i[o] = Ye(l, e[o], t[o], n[o]);
             return i;
         } else
             throw new Error(`Cannot spring ${typeof t} values`);
     }
 }
 
-function rt(l, e = {}) {
-    const t = Bl(l),
+function at(l, e = {}) {
+    const t = Pl(l),
         {
             stiffness: n = 0.15,
             damping: i = 0.8,
-            precision: s = 0.01
+            precision: o = 0.01
         } = e;
-    let o, r, a, f = l,
-        _ = l,
+    let s, f, a, _ = l,
+        r = l,
         u = 1,
         c = 0,
         m = !1;
 
-    function y(T, L = {}) {
-        _ = T;
-        const C = a = {};
-        return l == null || L.hard || S.stiffness >= 1 && S.damping >= 1 ? (m = !0, o = _t(), f = T, t.set(l = _), Promise.resolve()) : (L.soft && (c = 1 / ((L.soft === !0 ? 0.5 : +L.soft) * 60), u = 0), r || (o = _t(), m = !1, r = Vl((d) => {
+    function k(S, T = {}) {
+        r = S;
+        const y = a = {};
+        return l == null || T.hard || L.stiffness >= 1 && L.damping >= 1 ? (m = !0, s = st(), _ = S, t.set(l = r), Promise.resolve()) : (T.soft && (c = 1 / ((T.soft === !0 ? 0.5 : +T.soft) * 60), u = 0), f || (s = st(), m = !1, f = Bl((d) => {
             if (m)
-                return m = !1, r = null, !1;
+                return m = !1, f = null, !1;
             u = Math.min(u + c, 1);
-            const p = {
+            const C = {
                     inv_mass: u,
-                    opts: S,
+                    opts: L,
                     settled: !0,
-                    dt: (d - o) * 60 / 1e3
+                    dt: (d - s) * 60 / 1e3
                 },
-                H = We(p, f, l, _);
-            return o = d, f = l, t.set(l = H), p.settled && (r = null), !p.settled;
+                j = Ye(C, _, l, r);
+            return s = d, _ = l, t.set(l = j), C.settled && (f = null), !C.settled;
         })), new Promise((d) => {
-            r.promise.then(() => {
-                C === a && d();
+            f.promise.then(() => {
+                y === a && d();
             });
         }));
     }
-    const S = {
-        set: y,
-        update: (T, L) => y(T(_, l), L),
+    const L = {
+        set: k,
+        update: (S, T) => k(S(r, l), T),
         subscribe: t.subscribe,
         stiffness: n,
         damping: i,
-        precision: s
+        precision: o
+    };
+    return L;
+}
+const {
+    SvelteComponent: Zl,
+    append: Ol,
+    attr: le,
+    detach: Al,
+    init: Wl,
+    insert: Il,
+    noop: We,
+    safe_not_equal: Ul,
+    svg_element: rt
+} = window.__gradio__svelte__internal;
+
+function Xl(l) {
+    let e, t;
+    return {
+        c() {
+            e = rt("svg"), t = rt("polyline"), le(t, "points", "20 6 9 17 4 12"), le(e, "xmlns", "http://www.w3.org/2000/svg"), le(e, "viewBox", "2 0 20 20"), le(e, "fill", "none"), le(e, "stroke", "currentColor"), le(e, "stroke-width", "3"), le(e, "stroke-linecap", "round"), le(e, "stroke-linejoin", "round");
+        },
+        m(n, i) {
+            Il(n, e, i), Ol(e, t);
+        },
+        p: We,
+        i: We,
+        o: We,
+        d(n) {
+            n && Al(e);
+        }
+    };
+}
+class il extends Zl {
+    constructor(e) {
+        super(), Wl(this, e, null, Xl, Ul, {});
+    }
+}
+const {
+    SvelteComponent: Yl,
+    append: ut,
+    attr: re,
+    detach: Gl,
+    init: Jl,
+    insert: Kl,
+    noop: Ie,
+    safe_not_equal: Ql,
+    svg_element: Ue
+} = window.__gradio__svelte__internal;
+
+function xl(l) {
+    let e, t, n;
+    return {
+        c() {
+            e = Ue("svg"), t = Ue("path"), n = Ue("path"), re(t, "fill", "currentColor"), re(t, "d", "M28 10v18H10V10h18m0-2H10a2 2 0 0 0-2 2v18a2 2 0 0 0 2 2h18a2 2 0 0 0 2-2V10a2 2 0 0 0-2-2Z"), re(n, "fill", "currentColor"), re(n, "d", "M4 18H2V4a2 2 0 0 1 2-2h14v2H4Z"), re(e, "xmlns", "http://www.w3.org/2000/svg"), re(e, "viewBox", "0 0 33 33"), re(e, "color", "currentColor");
+        },
+        m(i, o) {
+            Kl(i, e, o), ut(e, t), ut(e, n);
+        },
+        p: Ie,
+        i: Ie,
+        o: Ie,
+        d(i) {
+            i && Gl(e);
+        }
+    };
+}
+class $l extends Yl {
+    constructor(e) {
+        super(), Jl(this, e, null, xl, Ql, {});
+    }
+}
+const {
+    SvelteComponent: en,
+    add_render_callback: tn,
+    append: ln,
+    attr: ue,
+    check_outros: nn,
+    create_bidirectional_transition: ct,
+    create_component: ol,
+    destroy_component: sl,
+    detach: fl,
+    element: _l,
+    group_outros: on,
+    init: sn,
+    insert: al,
+    listen: fn,
+    mount_component: rl,
+    safe_not_equal: _n,
+    space: an,
+    toggle_class: dt,
+    transition_in: Fe,
+    transition_out: De
+} = window.__gradio__svelte__internal, {
+    onDestroy: rn
+} = window.__gradio__svelte__internal;
+
+function mt(l) {
+    let e, t, n, i;
+    return t = new il({}), {
+        c() {
+            e = _l("span"), ol(t.$$.fragment), ue(e, "class", "check svelte-qjb524"), ue(e, "aria-roledescription", "Value copied"), ue(e, "aria-label", "Copied");
+        },
+        m(o, s) {
+            al(o, e, s), rl(t, e, null), i = !0;
+        },
+        i(o) {
+            i || (Fe(t.$$.fragment, o), o && tn(() => {
+                i && (n || (n = ct(e, ft, {}, !0)), n.run(1));
+            }), i = !0);
+        },
+        o(o) {
+            De(t.$$.fragment, o), o && (n || (n = ct(e, ft, {}, !1)), n.run(0)), i = !1;
+        },
+        d(o) {
+            o && fl(e), sl(t), o && n && n.end();
+        }
+    };
+}
+
+function un(l) {
+    let e, t, n, i, o, s;
+    t = new $l({});
+    let f = (
+        /*copied*/
+        l[0] && mt()
+    );
+    return {
+        c() {
+            e = _l("button"), ol(t.$$.fragment), n = an(), f && f.c(), ue(e, "title", "Copy text to clipboard"), ue(e, "aria-roledescription", "Copy value"), ue(e, "aria-label", "Copy"), ue(e, "class", "svelte-qjb524"), dt(
+                e,
+                "copied",
+                /*copied*/
+                l[0]
+            );
+        },
+        m(a, _) {
+            al(a, e, _), rl(t, e, null), ln(e, n), f && f.m(e, null), i = !0, o || (s = fn(
+                e,
+                "click",
+                /*handle_copy*/
+                l[1]
+            ), o = !0);
+        },
+        p(a, [_]) {
+            /*copied*/
+            a[0] ? f ? _ & /*copied*/
+                1 && Fe(f, 1) : (f = mt(), f.c(), Fe(f, 1), f.m(e, null)) : f && (on(), De(f, 1, 1, () => {
+                    f = null;
+                }), nn()), (!i || _ & /*copied*/
+                    1) && dt(
+                    e,
+                    "copied",
+                    /*copied*/
+                    a[0]
+                );
+        },
+        i(a) {
+            i || (Fe(t.$$.fragment, a), Fe(f), i = !0);
+        },
+        o(a) {
+            De(t.$$.fragment, a), De(f), i = !1;
+        },
+        d(a) {
+            a && fl(e), sl(t), f && f.d(), o = !1, s();
+        }
     };
-    return S;
 }
-const ut = [
+
+function cn(l, e, t) {
+    let n = !1,
+        {
+            value: i
+        } = e,
+        o;
+
+    function s() {
+        t(0, n = !0), o && clearTimeout(o), o = setTimeout(
+            () => {
+                t(0, n = !1);
+            },
+            2e3
+        );
+    }
+    async function f() {
+        "clipboard" in navigator && (await navigator.clipboard.writeText(i), s());
+    }
+    return rn(() => {
+        o && clearTimeout(o);
+    }), l.$$set = (a) => {
+        "value" in a && t(2, i = a.value);
+    }, [n, f, i];
+}
+class dn extends en {
+    constructor(e) {
+        super(), sn(this, e, cn, un, _n, {
+            value: 2
+        });
+    }
+}
+const {
+    SvelteComponent: mn,
+    attr: Ve,
+    create_component: gn,
+    destroy_component: hn,
+    detach: bn,
+    element: wn,
+    init: vn,
+    insert: pn,
+    listen: kn,
+    mount_component: yn,
+    noop: Cn,
+    safe_not_equal: qn,
+    transition_in: Tn,
+    transition_out: Sn
+} = window.__gradio__svelte__internal, {
+    createEventDispatcher: Ln
+} = window.__gradio__svelte__internal;
+
+function jn(l) {
+    let e, t, n, i, o;
+    return t = new il({}), {
+        c() {
+            e = wn("button"), gn(t.$$.fragment), Ve(e, "title", "Remove highlights"), Ve(e, "aria-roledescription", "Remove highlights"), Ve(e, "aria-label", "Remove highlights"), Ve(e, "class", "svelte-1ga0gmr");
+        },
+        m(s, f) {
+            pn(s, e, f), yn(t, e, null), n = !0, i || (o = kn(
+                e,
+                "click",
+                /*click_handler*/
+                l[1]
+            ), i = !0);
+        },
+        p: Cn,
+        i(s) {
+            n || (Tn(t.$$.fragment, s), n = !0);
+        },
+        o(s) {
+            Sn(t.$$.fragment, s), n = !1;
+        },
+        d(s) {
+            s && bn(e), hn(t), i = !1, o();
+        }
+    };
+}
+
+function Fn(l) {
+    const e = Ln();
+    return [e, () => e("click")];
+}
+class Hn extends mn {
+    constructor(e) {
+        super(), vn(this, e, Fn, jn, qn, {});
+    }
+}
+const {
+    SvelteComponent: Mn,
+    append: Nn,
+    attr: Vn,
+    check_outros: gt,
+    create_component: ul,
+    destroy_component: cl,
+    detach: zn,
+    element: En,
+    group_outros: ht,
+    init: Rn,
+    insert: Dn,
+    mount_component: dl,
+    noop: Bn,
+    safe_not_equal: Pn,
+    space: Zn,
+    transition_in: ie,
+    transition_out: pe
+} = window.__gradio__svelte__internal, {
+    createEventDispatcher: On
+} = window.__gradio__svelte__internal;
+
+function bt(l) {
+    let e, t;
+    return e = new Hn({}), e.$on(
+        "click",
+        /*removeTags*/
+        l[3]
+    ), {
+        c() {
+            ul(e.$$.fragment);
+        },
+        m(n, i) {
+            dl(e, n, i), t = !0;
+        },
+        p: Bn,
+        i(n) {
+            t || (ie(e.$$.fragment, n), t = !0);
+        },
+        o(n) {
+            pe(e.$$.fragment, n), t = !1;
+        },
+        d(n) {
+            cl(e, n);
+        }
+    };
+}
+
+function wt(l) {
+    let e, t;
+    return e = new dn({
+        props: {
+            value: (
+                /*value*/
+                l[0]
+            )
+        }
+    }), {
+        c() {
+            ul(e.$$.fragment);
+        },
+        m(n, i) {
+            dl(e, n, i), t = !0;
+        },
+        p(n, i) {
+            const o = {};
+            i & /*value*/
+                1 && (o.value = /*value*/
+                    n[0]), e.$set(o);
+        },
+        i(n) {
+            t || (ie(e.$$.fragment, n), t = !0);
+        },
+        o(n) {
+            pe(e.$$.fragment, n), t = !1;
+        },
+        d(n) {
+            cl(e, n);
+        }
+    };
+}
+
+function An(l) {
+    let e, t, n, i = (
+            /*show_remove_tags_button*/
+            l[2] && bt(l)
+        ),
+        o = (
+            /*show_copy_button*/
+            l[1] && wt(l)
+        );
+    return {
+        c() {
+            e = En("div"), i && i.c(), t = Zn(), o && o.c(), Vn(e, "class", "svelte-1bqqv16");
+        },
+        m(s, f) {
+            Dn(s, e, f), i && i.m(e, null), Nn(e, t), o && o.m(e, null), n = !0;
+        },
+        p(s, [f]) {
+            /*show_remove_tags_button*/
+            s[2] ? i ? (i.p(s, f), f & /*show_remove_tags_button*/
+                    4 && ie(i, 1)) : (i = bt(s), i.c(), ie(i, 1), i.m(e, t)) : i && (ht(), pe(i, 1, 1, () => {
+                    i = null;
+                }), gt()), /*show_copy_button*/
+                s[1] ? o ? (o.p(s, f), f & /*show_copy_button*/
+                    2 && ie(o, 1)) : (o = wt(s), o.c(), ie(o, 1), o.m(e, null)) : o && (ht(), pe(o, 1, 1, () => {
+                    o = null;
+                }), gt());
+        },
+        i(s) {
+            n || (ie(i), ie(o), n = !0);
+        },
+        o(s) {
+            pe(i), pe(o), n = !1;
+        },
+        d(s) {
+            s && zn(e), i && i.d(), o && o.d();
+        }
+    };
+}
+
+function Wn(l, e, t) {
+    let {
+        value: n
+    } = e, {
+        show_copy_button: i = !1
+    } = e, {
+        show_remove_tags_button: o = !1
+    } = e;
+    const s = On();
+
+    function f() {
+        s("removeTags");
+    }
+    return l.$$set = (a) => {
+        "value" in a && t(0, n = a.value), "show_copy_button" in a && t(1, i = a.show_copy_button), "show_remove_tags_button" in a && t(2, o = a.show_remove_tags_button);
+    }, [n, i, o, f];
+}
+class In extends Mn {
+    constructor(e) {
+        super(), Rn(this, e, Wn, An, Pn, {
+            value: 0,
+            show_copy_button: 1,
+            show_remove_tags_button: 2
+        });
+    }
+}
+const vt = [
         "red",
         "green",
         "blue",
         "yellow",
         "purple",
         "teal",
         "orange",
         "cyan",
         "lime",
         "pink"
     ],
-    El = [{
+    Un = [{
         color: "red",
         primary: 600,
         secondary: 100
     }, {
         color: "green",
         primary: 600,
         secondary: 100
@@ -573,15 +903,15 @@
         primary: 500,
         secondary: 100
     }, {
         color: "pink",
         primary: 600,
         secondary: 100
     }],
-    ct = {
+    pt = {
         inherit: "inherit",
         current: "currentColor",
         transparent: "transparent",
         black: "#000",
         white: "#fff",
         slate: {
             50: "#f8fafc",
@@ -866,357 +1196,263 @@
             600: "#e11d48",
             700: "#be123c",
             800: "#9f1239",
             900: "#881337",
             950: "#4c0519"
         }
     },
-    dt = El.reduce(
+    kt = Un.reduce(
         (l, {
             color: e,
             primary: t,
             secondary: n
         }) => ({
             ...l,
             [e]: {
-                primary: ct[e][t],
-                secondary: ct[e][n]
+                primary: pt[e][t],
+                secondary: pt[e][n]
             }
         }), {}
     ),
-    Pl = (l) => ut[l % ut.length];
+    Xn = (l) => vt[l % vt.length];
 
-function mt(l, e, t) {
+function yt(l, e, t) {
     if (!t) {
         var n = document.createElement("canvas");
         t = n.getContext("2d");
     }
     t.fillStyle = l, t.fillRect(0, 0, 1, 1);
-    const [i, s, o] = t.getImageData(0, 0, 1, 1).data;
-    return t.clearRect(0, 0, 1, 1), `rgba(${i}, ${s}, ${o}, ${255 / e})`;
+    const [i, o, s] = t.getImageData(0, 0, 1, 1).data;
+    return t.clearRect(0, 0, 1, 1), `rgba(${i}, ${o}, ${s}, ${255 / e})`;
 }
 
-function Zl(l, e, t) {
+function Yn(l, e, t) {
     var n = {};
     for (const i in l) {
-        const s = l[i].trim();
-        s in dt ? n[i] = dt[s] : n[i] = {
-            primary: e ? mt(l[i], 1, t) : l[i],
-            secondary: e ? mt(l[i], 0.5, t) : l[i]
+        const o = l[i].trim();
+        o in kt ? n[i] = kt[o] : n[i] = {
+            primary: e ? yt(l[i], 1, t) : l[i],
+            secondary: e ? yt(l[i], 0.5, t) : l[i]
         };
     }
     return n;
 }
 
-function Ol(l, e) {
+function Gn(l, e) {
     let t = [],
         n = null,
         i = null;
-    for (const [s, o] of l)
-        e === "empty" && o === null || e === "equal" && i === o ? n = n ? n + s : s : (n !== null && t.push([n, i]), n = s, i = o);
+    for (const [o, s] of l)
+        e === "empty" && s === null || e === "equal" && i === s ? n = n ? n + o : o : (n !== null && t.push([n, i]), n = o, i = s);
     return n !== null && t.push([n, i]), t;
 }
 
-function Rl(l) {
+function Jn(l) {
     const e = window.getSelection();
     if (e.rangeCount > 0) {
         const t = document.createRange();
         return t.setStart(l, 0), e.anchorNode !== null && t.setEnd(e.anchorNode, e.anchorOffset), t.toString().length;
     }
     return -1;
 }
 
-function Al(l, e) {
+function Kn(l, e) {
     var t = document.createTreeWalker(l, NodeFilter.SHOW_TEXT),
         n = t.nextNode();
     if (!n || !n.textContent)
         return null;
     for (var i = n.textContent.length; i < e;)
         if (n = t.nextNode(), n && n.textContent)
             i += n.textContent.length;
         else
             return null;
-    var s = n.textContent.length - (i - e);
+    var o = n.textContent.length - (i - e);
     return {
         node: n,
-        offset: s
+        offset: o
     };
 }
 const {
-    SvelteComponent: Dl,
-    add_render_callback: Ge,
-    append: ht,
-    attr: B,
-    binding_callbacks: bt,
-    bubble: Se,
-    check_outros: Xt,
-    create_component: Je,
-    create_in_transition: Il,
-    destroy_component: Ke,
-    detach: de,
-    element: Me,
-    empty: Wl,
-    group_outros: Yt,
-    init: Ul,
-    insert: me,
-    listen: Y,
-    mount_component: Qe,
-    noop: Gt,
-    run_all: Xl,
-    safe_not_equal: Yl,
-    set_data: Gl,
-    space: gt,
-    text: Jl,
-    toggle_class: wt,
-    transition_in: ie,
-    transition_out: ce
+    SvelteComponent: Qn,
+    add_render_callback: ml,
+    append: Ct,
+    attr: X,
+    binding_callbacks: qt,
+    bubble: je,
+    create_component: Tt,
+    destroy_component: St,
+    detach: Pe,
+    element: Qe,
+    init: xn,
+    insert: Ze,
+    listen: x,
+    mount_component: Lt,
+    run_all: $n,
+    safe_not_equal: ei,
+    set_data: ti,
+    space: jt,
+    text: li,
+    toggle_class: Ft,
+    transition_in: Ht,
+    transition_out: Mt
 } = window.__gradio__svelte__internal, {
-    beforeUpdate: Kl,
-    afterUpdate: Ql,
-    createEventDispatcher: xl
+    beforeUpdate: ni,
+    afterUpdate: ii,
+    createEventDispatcher: oi
 } = window.__gradio__svelte__internal;
 
-function $l(l) {
+function si(l) {
     let e;
     return {
         c() {
-            e = Jl(
+            e = li(
                 /*label*/
                 l[0]
             );
         },
         m(t, n) {
-            me(t, e, n);
+            Ze(t, e, n);
         },
         p(t, n) {
             n[0] & /*label*/
-                1 && Gl(
+                1 && ti(
                     e,
                     /*label*/
                     t[0]
                 );
         },
         d(t) {
-            t && de(e);
-        }
-    };
-}
-
-function kt(l) {
-    let e, t, n, i;
-    const s = [tn, en],
-        o = [];
-
-    function r(a, f) {
-        return (
-            /*copied*/
-            a[13] ? 0 : 1
-        );
-    }
-    return e = r(l), t = o[e] = s[e](l), {
-        c() {
-            t.c(), n = Wl();
-        },
-        m(a, f) {
-            o[e].m(a, f), me(a, n, f), i = !0;
-        },
-        p(a, f) {
-            let _ = e;
-            e = r(a), e === _ ? o[e].p(a, f) : (Yt(), ce(o[_], 1, 1, () => {
-                o[_] = null;
-            }), Xt(), t = o[e], t ? t.p(a, f) : (t = o[e] = s[e](a), t.c()), ie(t, 1), t.m(n.parentNode, n));
-        },
-        i(a) {
-            i || (ie(t), i = !0);
-        },
-        o(a) {
-            ce(t), i = !1;
-        },
-        d(a) {
-            a && de(n), o[e].d(a);
+            t && Pe(e);
         }
     };
 }
 
-function en(l) {
-    let e, t, n, i, s;
-    return t = new Ml({}), {
-        c() {
-            e = Me("button"), Je(t.$$.fragment), B(e, "aria-label", "Copy"), B(e, "aria-roledescription", "Copy text"), B(e, "class", "svelte-40uavx");
-        },
-        m(o, r) {
-            me(o, e, r), Qe(t, e, null), n = !0, i || (s = Y(
-                e,
-                "click",
-                /*handle_copy*/
-                l[15]
-            ), i = !0);
-        },
-        p: Gt,
-        i(o) {
-            n || (ie(t.$$.fragment, o), n = !0);
-        },
-        o(o) {
-            ce(t.$$.fragment, o), n = !1;
-        },
-        d(o) {
-            o && de(e), Ke(t), i = !1, s();
-        }
-    };
-}
-
-function tn(l) {
-    let e, t, n, i;
-    return t = new Cl({}), {
-        c() {
-            e = Me("button"), Je(t.$$.fragment), B(e, "aria-label", "Copied"), B(e, "aria-roledescription", "Text copied"), B(e, "class", "svelte-40uavx");
-        },
-        m(s, o) {
-            me(s, e, o), Qe(t, e, null), i = !0;
-        },
-        p: Gt,
-        i(s) {
-            i || (ie(t.$$.fragment, s), s && (n || Ge(() => {
-                n = Il(e, zl, {
-                    duration: 300
-                }), n.start();
-            })), i = !0);
-        },
-        o(s) {
-            ce(t.$$.fragment, s), i = !1;
-        },
-        d(s) {
-            s && de(e), Ke(t);
-        }
-    };
-}
-
-function ln(l) {
+function fi(l) {
     let e, t, n;
     return {
         c() {
-            e = Me("div"), B(e, "class", "textfield svelte-40uavx"), B(e, "data-testid", "highlighted-textbox"), B(e, "contenteditable", "true"), /*el_text*/
-                (l[10] === void 0 || /*marked_el_text*/
-                    l[11] === void 0) && Ge(() => (
+            e = Qe("div"), X(e, "class", "textfield svelte-1atky07"), X(e, "data-testid", "highlighted-textbox"), X(e, "contenteditable", "true"), X(e, "role", "textbox"), X(e, "tabindex", "0"), /*el_text*/
+                (l[11] === void 0 || /*marked_el_text*/
+                    l[12] === void 0) && ml(() => (
                     /*div_input_handler_1*/
-                    l[27].call(e)
+                    l[29].call(e)
                 ));
         },
-        m(i, s) {
-            me(i, e, s), l[26](e), /*el_text*/
-                l[10] !== void 0 && (e.textContent = /*el_text*/
-                    l[10]), /*marked_el_text*/
-                l[11] !== void 0 && (e.innerHTML = /*marked_el_text*/
-                    l[11]), t || (n = [
-                    Y(
+        m(i, o) {
+            Ze(i, e, o), l[28](e), /*el_text*/
+                l[11] !== void 0 && (e.textContent = /*el_text*/
+                    l[11]), /*marked_el_text*/
+                l[12] !== void 0 && (e.innerHTML = /*marked_el_text*/
+                    l[12]), t || (n = [
+                    x(
                         e,
                         "input",
                         /*div_input_handler_1*/
-                        l[27]
+                        l[29]
                     ),
-                    Y(
+                    x(
                         e,
                         "blur",
                         /*blur_handler*/
-                        l[19]
+                        l[21]
                     ),
-                    Y(
+                    x(
                         e,
                         "keypress",
                         /*keypress_handler*/
-                        l[20]
+                        l[22]
                     ),
-                    Y(
+                    x(
                         e,
                         "select",
                         /*select_handler*/
-                        l[21]
+                        l[23]
                     ),
-                    Y(
+                    x(
                         e,
                         "scroll",
                         /*scroll_handler*/
-                        l[22]
+                        l[24]
                     ),
-                    Y(
+                    x(
                         e,
                         "input",
                         /*handle_change*/
-                        l[14]
+                        l[16]
                     ),
-                    Y(
+                    x(
                         e,
                         "focus",
                         /*focus_handler*/
-                        l[23]
+                        l[25]
                     ),
-                    Y(
+                    x(
                         e,
                         "change",
                         /*handle_change*/
-                        l[14]
+                        l[16]
                     )
                 ], t = !0);
         },
-        p(i, s) {
-            s[0] & /*el_text*/
-                1024 && /*el_text*/
-                i[10] !== e.textContent && (e.textContent = /*el_text*/
-                    i[10]), s[0] & /*marked_el_text*/
-                2048 && /*marked_el_text*/
-                i[11] !== e.innerHTML && (e.innerHTML = /*marked_el_text*/
-                    i[11]);
+        p(i, o) {
+            o[0] & /*el_text*/
+                2048 && /*el_text*/
+                i[11] !== e.textContent && (e.textContent = /*el_text*/
+                    i[11]), o[0] & /*marked_el_text*/
+                4096 && /*marked_el_text*/
+                i[12] !== e.innerHTML && (e.innerHTML = /*marked_el_text*/
+                    i[12]);
         },
         d(i) {
-            i && de(e), l[26](null), t = !1, Xl(n);
+            i && Pe(e), l[28](null), t = !1, $n(n);
         }
     };
 }
 
-function nn(l) {
+function _i(l) {
     let e, t, n;
     return {
         c() {
-            e = Me("div"), B(e, "class", "textfield svelte-40uavx"), B(e, "data-testid", "highlighted-textbox"), B(e, "contenteditable", "false"), /*el_text*/
-                (l[10] === void 0 || /*marked_el_text*/
-                    l[11] === void 0) && Ge(() => (
+            e = Qe("div"), X(e, "class", "textfield svelte-1atky07"), X(e, "data-testid", "highlighted-textbox"), X(e, "contenteditable", "false"), /*el_text*/
+                (l[11] === void 0 || /*marked_el_text*/
+                    l[12] === void 0) && ml(() => (
                     /*div_input_handler*/
-                    l[25].call(e)
+                    l[27].call(e)
                 ));
         },
-        m(i, s) {
-            me(i, e, s), l[24](e), /*el_text*/
-                l[10] !== void 0 && (e.textContent = /*el_text*/
-                    l[10]), /*marked_el_text*/
-                l[11] !== void 0 && (e.innerHTML = /*marked_el_text*/
-                    l[11]), t || (n = Y(
+        m(i, o) {
+            Ze(i, e, o), l[26](e), /*el_text*/
+                l[11] !== void 0 && (e.textContent = /*el_text*/
+                    l[11]), /*marked_el_text*/
+                l[12] !== void 0 && (e.innerHTML = /*marked_el_text*/
+                    l[12]), t || (n = x(
                     e,
                     "input",
                     /*div_input_handler*/
-                    l[25]
+                    l[27]
                 ), t = !0);
         },
-        p(i, s) {
-            s[0] & /*el_text*/
-                1024 && /*el_text*/
-                i[10] !== e.textContent && (e.textContent = /*el_text*/
-                    i[10]), s[0] & /*marked_el_text*/
-                2048 && /*marked_el_text*/
-                i[11] !== e.innerHTML && (e.innerHTML = /*marked_el_text*/
-                    i[11]);
+        p(i, o) {
+            o[0] & /*el_text*/
+                2048 && /*el_text*/
+                i[11] !== e.textContent && (e.textContent = /*el_text*/
+                    i[11]), o[0] & /*marked_el_text*/
+                4096 && /*marked_el_text*/
+                i[12] !== e.innerHTML && (e.innerHTML = /*marked_el_text*/
+                    i[12]);
         },
         d(i) {
-            i && de(e), l[24](null), t = !1, n();
+            i && Pe(e), l[26](null), t = !1, n();
         }
     };
 }
 
-function sn(l) {
-    let e, t, n, i, s;
-    t = new hl({
+function ai(l) {
+    let e, t, n, i, o, s;
+    t = new El({
         props: {
             show_label: (
                 /*show_label*/
                 l[3]
             ),
             show_legend: (
                 /*show_legend*/
@@ -1228,370 +1464,388 @@
             ),
             legend_label: (
                 /*legend_label*/
                 l[1]
             ),
             _color_map: (
                 /*_color_map*/
-                l[12]
+                l[13]
             ),
             info: (
                 /*info*/
                 l[2]
             ),
             $$slots: {
-                default: [$l]
+                default: [si]
             },
             $$scope: {
                 ctx: l
             }
         }
-    });
-    let o = (
-        /*show_copy_button*/
-        l[7] && kt(l)
+    }), i = new In({
+        props: {
+            show_copy_button: (
+                /*show_copy_button*/
+                l[7]
+            ),
+            show_remove_tags_button: (
+                /*show_remove_tags_button*/
+                l[8] && ! /*tags_removed*/
+                l[14]
+            ),
+            value: (
+                /*tagged_text*/
+                l[15]
+            )
+        }
+    }), i.$on(
+        "removeTags",
+        /*handle_remove_tags*/
+        l[17]
     );
 
-    function r(_, u) {
+    function f(r, u) {
         return (
             /*disabled*/
-            _[8] ? nn : ln
+            r[9] ? _i : fi
         );
     }
-    let a = r(l),
-        f = a(l);
+    let a = f(l),
+        _ = a(l);
     return {
         c() {
-            e = Me("label"), Je(t.$$.fragment), n = gt(), o && o.c(), i = gt(), f.c(), B(e, "class", "svelte-40uavx"), wt(
+            e = Qe("label"), Tt(t.$$.fragment), n = jt(), Tt(i.$$.fragment), o = jt(), _.c(), X(e, "for", "highlighted-textbox"), X(e, "class", "svelte-1atky07"), Ft(
                 e,
                 "container",
                 /*container*/
                 l[6]
             );
         },
-        m(_, u) {
-            me(_, e, u), Qe(t, e, null), ht(e, n), o && o.m(e, null), ht(e, i), f.m(e, null), s = !0;
+        m(r, u) {
+            Ze(r, e, u), Lt(t, e, null), Ct(e, n), Lt(i, e, null), Ct(e, o), _.m(e, null), s = !0;
         },
-        p(_, u) {
+        p(r, u) {
             const c = {};
             u[0] & /*show_label*/
                 8 && (c.show_label = /*show_label*/
-                    _[3]), u[0] & /*show_legend*/
+                    r[3]), u[0] & /*show_legend*/
                 16 && (c.show_legend = /*show_legend*/
-                    _[4]), u[0] & /*show_legend_label*/
+                    r[4]), u[0] & /*show_legend_label*/
                 32 && (c.show_legend_label = /*show_legend_label*/
-                    _[5]), u[0] & /*legend_label*/
+                    r[5]), u[0] & /*legend_label*/
                 2 && (c.legend_label = /*legend_label*/
-                    _[1]), u[0] & /*_color_map*/
-                4096 && (c._color_map = /*_color_map*/
-                    _[12]), u[0] & /*info*/
+                    r[1]), u[0] & /*_color_map*/
+                8192 && (c._color_map = /*_color_map*/
+                    r[13]), u[0] & /*info*/
                 4 && (c.info = /*info*/
-                    _[2]), u[0] & /*label*/
+                    r[2]), u[0] & /*label*/
                 1 | u[1] & /*$$scope*/
-                256 && (c.$$scope = {
+                512 && (c.$$scope = {
                     dirty: u,
-                    ctx: _
-                }), t.$set(c), /*show_copy_button*/
-                _[7] ? o ? (o.p(_, u), u[0] & /*show_copy_button*/
-                    128 && ie(o, 1)) : (o = kt(_), o.c(), ie(o, 1), o.m(e, i)) : o && (Yt(), ce(o, 1, 1, () => {
-                    o = null;
-                }), Xt()), a === (a = r(_)) && f ? f.p(_, u) : (f.d(1), f = a(_), f && (f.c(), f.m(e, null))), (!s || u[0] & /*container*/
-                    64) && wt(
+                    ctx: r
+                }), t.$set(c);
+            const m = {};
+            u[0] & /*show_copy_button*/
+                128 && (m.show_copy_button = /*show_copy_button*/
+                    r[7]), u[0] & /*show_remove_tags_button, tags_removed*/
+                16640 && (m.show_remove_tags_button = /*show_remove_tags_button*/
+                    r[8] && ! /*tags_removed*/
+                    r[14]), u[0] & /*tagged_text*/
+                32768 && (m.value = /*tagged_text*/
+                    r[15]), i.$set(m), a === (a = f(r)) && _ ? _.p(r, u) : (_.d(1), _ = a(r), _ && (_.c(), _.m(e, null))), (!s || u[0] & /*container*/
+                    64) && Ft(
                     e,
                     "container",
                     /*container*/
-                    _[6]
+                    r[6]
                 );
         },
-        i(_) {
-            s || (ie(t.$$.fragment, _), ie(o), s = !0);
+        i(r) {
+            s || (Ht(t.$$.fragment, r), Ht(i.$$.fragment, r), s = !0);
         },
-        o(_) {
-            ce(t.$$.fragment, _), ce(o), s = !1;
+        o(r) {
+            Mt(t.$$.fragment, r), Mt(i.$$.fragment, r), s = !1;
         },
-        d(_) {
-            _ && de(e), Ke(t), o && o.d(), f.d();
+        d(r) {
+            r && Pe(e), St(t), St(i), _.d();
         }
     };
 }
 
-function on(l, e, t) {
+function ri(l, e, t) {
     const n = typeof document < "u";
     let {
         value: i = []
     } = e, {
-        value_is_output: s = !1
+        value_is_output: o = !1
     } = e, {
-        label: o
+        label: s
     } = e, {
-        legend_label: r
+        legend_label: f
     } = e, {
         info: a = void 0
     } = e, {
-        show_label: f = !0
+        show_label: _ = !0
     } = e, {
-        show_legend: _ = !1
+        show_legend: r = !1
     } = e, {
         show_legend_label: u = !1
     } = e, {
         container: c = !0
     } = e, {
         color_map: m = {}
     } = e, {
-        show_copy_button: y = !1
+        show_copy_button: k = !1
+    } = e, {
+        show_remove_tags_button: L = !1
     } = e, {
         disabled: S
-    } = e, T, L = "", C = "", d, p = !m || Object.keys(m).length === 0 ? {} : m, H = {}, b = !1, R;
+    } = e, T, y = "", d = "", C, j = !m || Object.keys(m).length === 0 ? {} : m, h = {}, Z = !1, J = "";
 
-    function K() {
-        for (let h in p)
-            i.map(([N, j]) => j).includes(h) || delete p[h];
+    function E() {
+        for (let g in j)
+            i.map(([M, F]) => F).includes(g) || delete j[g];
         if (i.length > 0) {
-            for (let [h, N] of i)
-                if (N !== null && !(N in p)) {
-                    let j = Pl(Object.keys(p).length);
-                    p[N] = j;
+            for (let [g, M] of i)
+                if (M !== null && !(M in j)) {
+                    let F = Xn(Object.keys(j).length);
+                    j[M] = F;
                 }
         }
-        t(12, H = Zl(p, n, d));
+        t(13, h = Yn(j, n, C));
     }
 
-    function E(h) {
-        i.length > 0 && h && (t(10, L = i.map(([N, j]) => N).join("")), t(11, C = i.map(([N, j]) => j !== null ? `<mark class="hl ${j}" style="background-color:${H[j].secondary}">${N}</mark>` : N).join("")));
+    function O(g) {
+        i.length > 0 && g && (t(11, y = i.map(([M, F]) => M).join("")), t(12, d = i.map(([M, F]) => F !== null ? `<mark class="hl ${F}" style="background-color:${h[F].secondary}">${M}</mark>` : M).join("")), t(15, J = i.map(([M, F]) => F !== null ? `<${F}>${M}</${F}>` : M).join("")));
     }
-    const A = xl();
-    Kl(() => {
+    const R = oi();
+    ni(() => {
         T && T.offsetHeight + T.scrollTop > T.scrollHeight - 100;
     });
 
-    function X() {
-        P(), he(), A("change", i), s || A("input", i);
+    function ae() {
+        D(), A(), R("change", i), o || R("input", i);
     }
-    Ql(() => {
-        K(), E(s), t(17, s = !1);
+    ii(() => {
+        E(), O(o), t(19, o = !1);
     });
 
-    function he() {
-        let h = [],
-            N = "",
-            j = null,
+    function A() {
+        let g = [],
+            M = "",
+            F = null,
             ee = !1,
-            we = "",
-            ke = C.replace(/&nbsp;|&amp;|&lt;|&gt;/g, function(te) {
+            be = "",
+            we = d.replace(/&nbsp;|&amp;|&lt;|&gt;/g, function(te) {
                 return {
                     "&nbsp;": " ",
                     "&amp;": "&",
                     "&lt;": "<",
                     "&gt;": ">"
                 } [te];
             });
-        for (let te = 0; te < ke.length; te++) {
-            let x = ke[te];
-            if (x === "<")
-                ee = !0, N && h.push([N, j]), N = "", j = null;
-            else if (x === ">") {
-                if (ee = !1, we.slice(0, 4) === "mark") {
-                    let Ve = /class="hl ([^"]+)"/.exec(we);
-                    j = Ve ? Ve[1] : null;
+        for (let te = 0; te < we.length; te++) {
+            let Q = we[te];
+            if (Q === "<")
+                ee = !0, M && g.push([M, F]), M = "", F = null;
+            else if (Q === ">") {
+                if (ee = !1, be.slice(0, 4) === "mark") {
+                    let Ne = /class="hl ([^"]+)"/.exec(be);
+                    F = Ne ? Ne[1] : null;
                 }
-                we = "";
+                be = "";
             } else
-                ee ? we += x : N += x;
+                ee ? be += Q : M += Q;
         }
-        N && h.push([N, j]), t(16, i = h);
-    }
-    async function D() {
-        "clipboard" in navigator && (await navigator.clipboard.writeText(L), Q());
+        M && g.push([M, F]), t(18, i = g);
     }
 
-    function Q() {
-        t(13, b = !0), R && clearTimeout(R), R = setTimeout(
-            () => {
-                t(13, b = !1);
-            },
-            1e3
-        );
+    function K() {
+        t(12, d = y), ae(), t(14, Z = !0), R("clear");
     }
 
-    function P() {
-        const h = window.getSelection(),
-            N = h.anchorOffset;
-        if (h.rangeCount > 0) {
-            var j = h.getRangeAt(0).commonAncestorContainer.parentElement;
-            if (j && j.tagName.toLowerCase() === "mark") {
-                const Ve = j.textContent;
-                var ee = j.parentElement,
-                    we = document.createTextNode(Ve);
-                ee.replaceChild(we, j), t(11, C = ee.innerHTML);
-                var ke = document.createRange(),
+    function D() {
+        const g = window.getSelection(),
+            M = g.anchorOffset;
+        if (g.rangeCount > 0) {
+            var F = g.getRangeAt(0).commonAncestorContainer.parentElement;
+            if (F && F.tagName.toLowerCase() === "mark") {
+                const Ne = F.textContent;
+                var ee = F.parentElement,
+                    be = document.createTextNode(Ne);
+                ee.replaceChild(be, F), t(12, d = ee.innerHTML);
+                var we = document.createRange(),
                     te = window.getSelection();
-                const tl = N + Rl(ee);
-                var x = Al(ee, tl);
-                ke.setStart(x.node, x.offset), ke.setEnd(x.node, x.offset), te.removeAllRanges(), te.addRange(ke);
+                const kl = M + Jn(ee);
+                var Q = Kn(ee, kl);
+                we.setStart(Q.node, Q.offset), we.setEnd(Q.node, Q.offset), te.removeAllRanges(), te.addRange(we);
             }
         }
     }
 
-    function be(h) {
-        Se.call(this, l, h);
+    function me(g) {
+        je.call(this, l, g);
     }
 
-    function g(h) {
-        Se.call(this, l, h);
+    function Le(g) {
+        je.call(this, l, g);
     }
 
-    function je(h) {
-        Se.call(this, l, h);
+    function ge(g) {
+        je.call(this, l, g);
     }
 
-    function Ne(h) {
-        Se.call(this, l, h);
+    function b(g) {
+        je.call(this, l, g);
     }
 
-    function ge(h) {
-        Se.call(this, l, h);
+    function he(g) {
+        je.call(this, l, g);
     }
 
-    function Ze(h) {
-        bt[h ? "unshift" : "push"](() => {
-            T = h, t(9, T);
+    function Oe(g) {
+        qt[g ? "unshift" : "push"](() => {
+            T = g, t(10, T);
         });
     }
 
-    function Oe() {
-        L = this.textContent, C = this.innerHTML, t(10, L), t(11, C);
+    function Ae() {
+        y = this.textContent, d = this.innerHTML, t(11, y), t(12, d);
     }
 
-    function w(h) {
-        bt[h ? "unshift" : "push"](() => {
-            T = h, t(9, T);
+    function w(g) {
+        qt[g ? "unshift" : "push"](() => {
+            T = g, t(10, T);
         });
     }
 
-    function el() {
-        L = this.textContent, C = this.innerHTML, t(10, L), t(11, C);
+    function pl() {
+        y = this.textContent, d = this.innerHTML, t(11, y), t(12, d);
     }
-    return l.$$set = (h) => {
-        "value" in h && t(16, i = h.value), "value_is_output" in h && t(17, s = h.value_is_output), "label" in h && t(0, o = h.label), "legend_label" in h && t(1, r = h.legend_label), "info" in h && t(2, a = h.info), "show_label" in h && t(3, f = h.show_label), "show_legend" in h && t(4, _ = h.show_legend), "show_legend_label" in h && t(5, u = h.show_legend_label), "container" in h && t(6, c = h.container), "color_map" in h && t(18, m = h.color_map), "show_copy_button" in h && t(7, y = h.show_copy_button), "disabled" in h && t(8, S = h.disabled);
-    }, K(), E(!0), [
-        o,
-        r,
-        a,
+    return l.$$set = (g) => {
+        "value" in g && t(18, i = g.value), "value_is_output" in g && t(19, o = g.value_is_output), "label" in g && t(0, s = g.label), "legend_label" in g && t(1, f = g.legend_label), "info" in g && t(2, a = g.info), "show_label" in g && t(3, _ = g.show_label), "show_legend" in g && t(4, r = g.show_legend), "show_legend_label" in g && t(5, u = g.show_legend_label), "container" in g && t(6, c = g.container), "color_map" in g && t(20, m = g.color_map), "show_copy_button" in g && t(7, k = g.show_copy_button), "show_remove_tags_button" in g && t(8, L = g.show_remove_tags_button), "disabled" in g && t(9, S = g.disabled);
+    }, E(), O(!0), [
+        s,
         f,
+        a,
         _,
+        r,
         u,
         c,
-        y,
+        k,
+        L,
         S,
         T,
-        L,
-        C,
-        H,
-        b,
-        X,
-        D,
+        y,
+        d,
+        h,
+        Z,
+        J,
+        ae,
+        K,
         i,
-        s,
+        o,
         m,
-        be,
-        g,
-        je,
-        Ne,
+        me,
+        Le,
         ge,
-        Ze,
+        b,
+        he,
         Oe,
+        Ae,
         w,
-        el
+        pl
     ];
 }
-class fn extends Dl {
+class ui extends Qn {
     constructor(e) {
-        super(), Ul(
+        super(), xn(
             this,
             e,
-            on,
-            sn,
-            Yl, {
-                value: 16,
-                value_is_output: 17,
+            ri,
+            ai,
+            ei, {
+                value: 18,
+                value_is_output: 19,
                 label: 0,
                 legend_label: 1,
                 info: 2,
                 show_label: 3,
                 show_legend: 4,
                 show_legend_label: 5,
                 container: 6,
-                color_map: 18,
+                color_map: 20,
                 show_copy_button: 7,
-                disabled: 8
+                show_remove_tags_button: 8,
+                disabled: 9
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: _n,
-    assign: an,
-    create_slot: rn,
-    detach: un,
-    element: cn,
-    get_all_dirty_from_scope: dn,
-    get_slot_changes: mn,
-    get_spread_update: hn,
-    init: bn,
-    insert: gn,
-    safe_not_equal: wn,
-    set_dynamic_element_data: vt,
+    SvelteComponent: ci,
+    assign: di,
+    create_slot: mi,
+    detach: gi,
+    element: hi,
+    get_all_dirty_from_scope: bi,
+    get_slot_changes: wi,
+    get_spread_update: vi,
+    init: pi,
+    insert: ki,
+    safe_not_equal: yi,
+    set_dynamic_element_data: Nt,
     set_style: z,
     toggle_class: ne,
-    transition_in: Jt,
-    transition_out: Kt,
-    update_slot_base: kn
+    transition_in: gl,
+    transition_out: hl,
+    update_slot_base: Ci
 } = window.__gradio__svelte__internal;
 
-function vn(l) {
+function qi(l) {
     let e, t, n;
     const i = (
             /*#slots*/
             l[18].default
         ),
-        s = rn(
+        o = mi(
             i,
             l,
             /*$$scope*/
             l[17],
             null
         );
-    let o = [{
+    let s = [{
             "data-testid": (
                 /*test_id*/
                 l[7]
             )
         }, {
             id: (
                 /*elem_id*/
                 l[2]
             )
         }, {
             class: t = "block " + /*elem_classes*/
                 l[3].join(" ") + " svelte-1t38q2d"
         }],
-        r = {};
-    for (let a = 0; a < o.length; a += 1)
-        r = an(r, o[a]);
+        f = {};
+    for (let a = 0; a < s.length; a += 1)
+        f = di(f, s[a]);
     return {
         c() {
-            e = cn(
+            e = hi(
                 /*tag*/
                 l[14]
-            ), s && s.c(), vt(
+            ), o && o.c(), Nt(
                 /*tag*/
                 l[14]
-            )(e, r), ne(
+            )(e, f), ne(
                 e,
                 "hidden",
                 /*visible*/
                 l[10] === !1
             ), ne(
                 e,
                 "padded",
@@ -1633,55 +1887,55 @@
                 e,
                 "flex-grow",
                 /*scale*/
                 l[12]
             ), z(e, "min-width", `calc(min(${/*min_width*/
       l[13]}px, 100%))`), z(e, "border-width", "var(--block-border-width)");
         },
-        m(a, f) {
-            gn(a, e, f), s && s.m(e, null), n = !0;
+        m(a, _) {
+            ki(a, e, _), o && o.m(e, null), n = !0;
         },
-        p(a, f) {
-            s && s.p && (!n || f & /*$$scope*/
-                    131072) && kn(
-                    s,
+        p(a, _) {
+            o && o.p && (!n || _ & /*$$scope*/
+                    131072) && Ci(
+                    o,
                     i,
                     a,
                     /*$$scope*/
                     a[17],
-                    n ? mn(
+                    n ? wi(
                         i,
                         /*$$scope*/
                         a[17],
-                        f,
+                        _,
                         null
-                    ) : dn(
+                    ) : bi(
                         /*$$scope*/
                         a[17]
                     ),
                     null
-                ), vt(
+                ), Nt(
                     /*tag*/
                     a[14]
-                )(e, r = hn(o, [
-                    (!n || f & /*test_id*/
+                )(e, f = vi(s, [
+                    (!n || _ & /*test_id*/
                         128) && {
                         "data-testid": (
                             /*test_id*/
                             a[7]
                         )
                     },
-                    (!n || f & /*elem_id*/
+                    (!n || _ & /*elem_id*/
                         4) && {
                         id: (
                             /*elem_id*/
                             a[2]
                         )
                     },
-                    (!n || f & /*elem_classes*/
+                    (!n || _ & /*elem_classes*/
                         8 && t !== (t = "block " + /*elem_classes*/
                             a[3].join(" ") + " svelte-1t38q2d")) && {
                         class: t
                     }
                 ])), ne(
                     e,
                     "hidden",
@@ -1695,163 +1949,163 @@
                 ), ne(
                     e,
                     "border_focus",
                     /*border_mode*/
                     a[5] === "focus"
                 ), ne(e, "hide-container", ! /*explicit_call*/
                     a[8] && ! /*container*/
-                    a[9]), f & /*height*/
+                    a[9]), _ & /*height*/
                 1 && z(
                     e,
                     "height",
                     /*get_dimension*/
                     a[15](
                         /*height*/
                         a[0]
                     )
-                ), f & /*width*/
+                ), _ & /*width*/
                 2 && z(e, "width", typeof /*width*/ a[1] == "number" ? `calc(min(${/*width*/
       a[1]}px, 100%))` : (
                     /*get_dimension*/
                     a[15](
                         /*width*/
                         a[1]
                     )
-                )), f & /*variant*/
+                )), _ & /*variant*/
                 16 && z(
                     e,
                     "border-style",
                     /*variant*/
                     a[4]
-                ), f & /*allow_overflow*/
+                ), _ & /*allow_overflow*/
                 2048 && z(
                     e,
                     "overflow",
                     /*allow_overflow*/
                     a[11] ? "visible" : "hidden"
-                ), f & /*scale*/
+                ), _ & /*scale*/
                 4096 && z(
                     e,
                     "flex-grow",
                     /*scale*/
                     a[12]
-                ), f & /*min_width*/
+                ), _ & /*min_width*/
                 8192 && z(e, "min-width", `calc(min(${/*min_width*/
       a[13]}px, 100%))`);
         },
         i(a) {
-            n || (Jt(s, a), n = !0);
+            n || (gl(o, a), n = !0);
         },
         o(a) {
-            Kt(s, a), n = !1;
+            hl(o, a), n = !1;
         },
         d(a) {
-            a && un(e), s && s.d(a);
+            a && gi(e), o && o.d(a);
         }
     };
 }
 
-function pn(l) {
+function Ti(l) {
     let e, t = (
         /*tag*/
-        l[14] && vn(l)
+        l[14] && qi(l)
     );
     return {
         c() {
             t && t.c();
         },
         m(n, i) {
             t && t.m(n, i), e = !0;
         },
         p(n, [i]) {
             /*tag*/
             n[14] && t.p(n, i);
         },
         i(n) {
-            e || (Jt(t, n), e = !0);
+            e || (gl(t, n), e = !0);
         },
         o(n) {
-            Kt(t, n), e = !1;
+            hl(t, n), e = !1;
         },
         d(n) {
             t && t.d(n);
         }
     };
 }
 
-function yn(l, e, t) {
+function Si(l, e, t) {
     let {
         $$slots: n = {},
         $$scope: i
     } = e, {
-        height: s = void 0
+        height: o = void 0
     } = e, {
-        width: o = void 0
+        width: s = void 0
     } = e, {
-        elem_id: r = ""
+        elem_id: f = ""
     } = e, {
         elem_classes: a = []
     } = e, {
-        variant: f = "solid"
+        variant: _ = "solid"
     } = e, {
-        border_mode: _ = "base"
+        border_mode: r = "base"
     } = e, {
         padding: u = !0
     } = e, {
         type: c = "normal"
     } = e, {
         test_id: m = void 0
     } = e, {
-        explicit_call: y = !1
+        explicit_call: k = !1
     } = e, {
-        container: S = !0
+        container: L = !0
     } = e, {
-        visible: T = !0
+        visible: S = !0
     } = e, {
-        allow_overflow: L = !0
+        allow_overflow: T = !0
     } = e, {
-        scale: C = null
+        scale: y = null
     } = e, {
         min_width: d = 0
-    } = e, p = c === "fieldset" ? "fieldset" : "div";
-    const H = (b) => {
-        if (b !== void 0) {
-            if (typeof b == "number")
-                return b + "px";
-            if (typeof b == "string")
-                return b;
+    } = e, C = c === "fieldset" ? "fieldset" : "div";
+    const j = (h) => {
+        if (h !== void 0) {
+            if (typeof h == "number")
+                return h + "px";
+            if (typeof h == "string")
+                return h;
         }
     };
-    return l.$$set = (b) => {
-        "height" in b && t(0, s = b.height), "width" in b && t(1, o = b.width), "elem_id" in b && t(2, r = b.elem_id), "elem_classes" in b && t(3, a = b.elem_classes), "variant" in b && t(4, f = b.variant), "border_mode" in b && t(5, _ = b.border_mode), "padding" in b && t(6, u = b.padding), "type" in b && t(16, c = b.type), "test_id" in b && t(7, m = b.test_id), "explicit_call" in b && t(8, y = b.explicit_call), "container" in b && t(9, S = b.container), "visible" in b && t(10, T = b.visible), "allow_overflow" in b && t(11, L = b.allow_overflow), "scale" in b && t(12, C = b.scale), "min_width" in b && t(13, d = b.min_width), "$$scope" in b && t(17, i = b.$$scope);
+    return l.$$set = (h) => {
+        "height" in h && t(0, o = h.height), "width" in h && t(1, s = h.width), "elem_id" in h && t(2, f = h.elem_id), "elem_classes" in h && t(3, a = h.elem_classes), "variant" in h && t(4, _ = h.variant), "border_mode" in h && t(5, r = h.border_mode), "padding" in h && t(6, u = h.padding), "type" in h && t(16, c = h.type), "test_id" in h && t(7, m = h.test_id), "explicit_call" in h && t(8, k = h.explicit_call), "container" in h && t(9, L = h.container), "visible" in h && t(10, S = h.visible), "allow_overflow" in h && t(11, T = h.allow_overflow), "scale" in h && t(12, y = h.scale), "min_width" in h && t(13, d = h.min_width), "$$scope" in h && t(17, i = h.$$scope);
     }, [
-        s,
         o,
-        r,
-        a,
+        s,
         f,
+        a,
         _,
+        r,
         u,
         m,
-        y,
+        k,
+        L,
         S,
         T,
-        L,
-        C,
+        y,
         d,
-        p,
-        H,
+        C,
+        j,
         c,
         i,
         n
     ];
 }
-class Cn extends _n {
+class Li extends ci {
     constructor(e) {
-        super(), bn(this, e, yn, pn, wn, {
+        super(), pi(this, e, Si, Ti, yi, {
             height: 0,
             width: 1,
             elem_id: 2,
             elem_classes: 3,
             variant: 4,
             border_mode: 5,
             padding: 6,
@@ -1863,1153 +2117,1153 @@
             allow_overflow: 11,
             scale: 12,
             min_width: 13
         });
     }
 }
 
-function pe(l) {
+function ke(l) {
     let e = ["", "k", "M", "G", "T", "P", "E", "Z"],
         t = 0;
     for (; l > 1e3 && t < e.length - 1;)
         l /= 1e3, t++;
     let n = e[t];
     return (Number.isInteger(l) ? l : l.toFixed(1)) + n;
 }
 const {
-    SvelteComponent: qn,
-    append: I,
+    SvelteComponent: ji,
+    append: W,
     attr: q,
-    component_subscribe: pt,
-    detach: Tn,
-    element: Ln,
-    init: Sn,
-    insert: Fn,
-    noop: yt,
-    safe_not_equal: Hn,
+    component_subscribe: Vt,
+    detach: Fi,
+    element: Hi,
+    init: Mi,
+    insert: Ni,
+    noop: zt,
+    safe_not_equal: Vi,
     set_style: ze,
-    svg_element: W,
-    toggle_class: Ct
+    svg_element: I,
+    toggle_class: Et
 } = window.__gradio__svelte__internal, {
-    onMount: Mn
+    onMount: zi
 } = window.__gradio__svelte__internal;
 
-function jn(l) {
-    let e, t, n, i, s, o, r, a, f, _, u, c;
+function Ei(l) {
+    let e, t, n, i, o, s, f, a, _, r, u, c;
     return {
         c() {
-            e = Ln("div"), t = W("svg"), n = W("g"), i = W("path"), s = W("path"), o = W("path"), r = W("path"), a = W("g"), f = W("path"), _ = W("path"), u = W("path"), c = W("path"), q(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(s, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(s, "fill", "#FF7C00"), q(s, "class", "svelte-43sxxs"), q(o, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(o, "fill", "#FF7C00"), q(o, "fill-opacity", "0.4"), q(o, "class", "svelte-43sxxs"), q(r, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(r, "fill", "#FF7C00"), q(r, "class", "svelte-43sxxs"), ze(n, "transform", "translate(" + /*$top*/
+            e = Hi("div"), t = I("svg"), n = I("g"), i = I("path"), o = I("path"), s = I("path"), f = I("path"), a = I("g"), _ = I("path"), r = I("path"), u = I("path"), c = I("path"), q(i, "d", "M255.926 0.754768L509.702 139.936V221.027L255.926 81.8465V0.754768Z"), q(i, "fill", "#FF7C00"), q(i, "fill-opacity", "0.4"), q(i, "class", "svelte-43sxxs"), q(o, "d", "M509.69 139.936L254.981 279.641V361.255L509.69 221.55V139.936Z"), q(o, "fill", "#FF7C00"), q(o, "class", "svelte-43sxxs"), q(s, "d", "M0.250138 139.937L254.981 279.641V361.255L0.250138 221.55V139.937Z"), q(s, "fill", "#FF7C00"), q(s, "fill-opacity", "0.4"), q(s, "class", "svelte-43sxxs"), q(f, "d", "M255.923 0.232622L0.236328 139.936V221.55L255.923 81.8469V0.232622Z"), q(f, "fill", "#FF7C00"), q(f, "class", "svelte-43sxxs"), ze(n, "transform", "translate(" + /*$top*/
                 l[1][0] + "px, " + /*$top*/
-                l[1][1] + "px)"), q(f, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(f, "fill", "#FF7C00"), q(f, "fill-opacity", "0.4"), q(f, "class", "svelte-43sxxs"), q(_, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(_, "fill", "#FF7C00"), q(_, "class", "svelte-43sxxs"), q(u, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(u, "fill", "#FF7C00"), q(u, "fill-opacity", "0.4"), q(u, "class", "svelte-43sxxs"), q(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(c, "fill", "#FF7C00"), q(c, "class", "svelte-43sxxs"), ze(a, "transform", "translate(" + /*$bottom*/
+                l[1][1] + "px)"), q(_, "d", "M255.926 141.5L509.702 280.681V361.773L255.926 222.592V141.5Z"), q(_, "fill", "#FF7C00"), q(_, "fill-opacity", "0.4"), q(_, "class", "svelte-43sxxs"), q(r, "d", "M509.69 280.679L254.981 420.384V501.998L509.69 362.293V280.679Z"), q(r, "fill", "#FF7C00"), q(r, "class", "svelte-43sxxs"), q(u, "d", "M0.250138 280.681L254.981 420.386V502L0.250138 362.295V280.681Z"), q(u, "fill", "#FF7C00"), q(u, "fill-opacity", "0.4"), q(u, "class", "svelte-43sxxs"), q(c, "d", "M255.923 140.977L0.236328 280.68V362.294L255.923 222.591V140.977Z"), q(c, "fill", "#FF7C00"), q(c, "class", "svelte-43sxxs"), ze(a, "transform", "translate(" + /*$bottom*/
                 l[2][0] + "px, " + /*$bottom*/
-                l[2][1] + "px)"), q(t, "viewBox", "-1200 -1200 3000 3000"), q(t, "fill", "none"), q(t, "xmlns", "http://www.w3.org/2000/svg"), q(t, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), Ct(
+                l[2][1] + "px)"), q(t, "viewBox", "-1200 -1200 3000 3000"), q(t, "fill", "none"), q(t, "xmlns", "http://www.w3.org/2000/svg"), q(t, "class", "svelte-43sxxs"), q(e, "class", "svelte-43sxxs"), Et(
                 e,
                 "margin",
                 /*margin*/
                 l[0]
             );
         },
-        m(m, y) {
-            Fn(m, e, y), I(e, t), I(t, n), I(n, i), I(n, s), I(n, o), I(n, r), I(t, a), I(a, f), I(a, _), I(a, u), I(a, c);
+        m(m, k) {
+            Ni(m, e, k), W(e, t), W(t, n), W(n, i), W(n, o), W(n, s), W(n, f), W(t, a), W(a, _), W(a, r), W(a, u), W(a, c);
         },
-        p(m, [y]) {
-            y & /*$top*/
+        p(m, [k]) {
+            k & /*$top*/
                 2 && ze(n, "transform", "translate(" + /*$top*/
                     m[1][0] + "px, " + /*$top*/
-                    m[1][1] + "px)"), y & /*$bottom*/
+                    m[1][1] + "px)"), k & /*$bottom*/
                 4 && ze(a, "transform", "translate(" + /*$bottom*/
                     m[2][0] + "px, " + /*$bottom*/
-                    m[2][1] + "px)"), y & /*margin*/
-                1 && Ct(
+                    m[2][1] + "px)"), k & /*margin*/
+                1 && Et(
                     e,
                     "margin",
                     /*margin*/
                     m[0]
                 );
         },
-        i: yt,
-        o: yt,
+        i: zt,
+        o: zt,
         d(m) {
-            m && Tn(e);
+            m && Fi(e);
         }
     };
 }
 
-function Nn(l, e, t) {
+function Ri(l, e, t) {
     let n, i, {
-        margin: s = !0
+        margin: o = !0
     } = e;
-    const o = rt([0, 0]);
-    pt(l, o, (c) => t(1, n = c));
-    const r = rt([0, 0]);
-    pt(l, r, (c) => t(2, i = c));
+    const s = at([0, 0]);
+    Vt(l, s, (c) => t(1, n = c));
+    const f = at([0, 0]);
+    Vt(l, f, (c) => t(2, i = c));
     let a;
-    async function f() {
-        await Promise.all([o.set([125, 140]), r.set([-125, -140])]), await Promise.all([o.set([-125, 140]), r.set([125, -140])]), await Promise.all([o.set([-125, 0]), r.set([125, -0])]), await Promise.all([o.set([125, 0]), r.set([-125, 0])]);
-    }
     async function _() {
-        await f(), a || _();
+        await Promise.all([s.set([125, 140]), f.set([-125, -140])]), await Promise.all([s.set([-125, 140]), f.set([125, -140])]), await Promise.all([s.set([-125, 0]), f.set([125, -0])]), await Promise.all([s.set([125, 0]), f.set([-125, 0])]);
+    }
+    async function r() {
+        await _(), a || r();
     }
     async function u() {
-        await Promise.all([o.set([125, 0]), r.set([-125, 0])]), _();
+        await Promise.all([s.set([125, 0]), f.set([-125, 0])]), r();
     }
-    return Mn(() => (u(), () => a = !0)), l.$$set = (c) => {
-        "margin" in c && t(0, s = c.margin);
-    }, [s, n, i, o, r];
+    return zi(() => (u(), () => a = !0)), l.$$set = (c) => {
+        "margin" in c && t(0, o = c.margin);
+    }, [o, n, i, s, f];
 }
-class Vn extends qn {
+class Di extends ji {
     constructor(e) {
-        super(), Sn(this, e, Nn, jn, Hn, {
+        super(), Mi(this, e, Ri, Ei, Vi, {
             margin: 0
         });
     }
 }
 const {
-    SvelteComponent: zn,
-    append: re,
-    attr: G,
-    binding_callbacks: qt,
-    check_outros: Qt,
-    create_component: Bn,
-    create_slot: En,
-    destroy_component: Pn,
-    destroy_each: xt,
-    detach: k,
+    SvelteComponent: Bi,
+    append: ce,
+    attr: Y,
+    binding_callbacks: Rt,
+    check_outros: bl,
+    create_component: Pi,
+    create_slot: Zi,
+    destroy_component: Oi,
+    destroy_each: wl,
+    detach: v,
     element: $,
-    empty: Le,
-    ensure_array_like: Pe,
-    get_all_dirty_from_scope: Zn,
-    get_slot_changes: On,
-    group_outros: $t,
-    init: Rn,
-    insert: v,
-    mount_component: An,
-    noop: Ue,
-    safe_not_equal: Dn,
-    set_data: O,
-    set_style: se,
-    space: J,
-    text: F,
-    toggle_class: Z,
+    empty: Se,
+    ensure_array_like: Be,
+    get_all_dirty_from_scope: Ai,
+    get_slot_changes: Wi,
+    group_outros: vl,
+    init: Ii,
+    insert: p,
+    mount_component: Ui,
+    noop: Ge,
+    safe_not_equal: Xi,
+    set_data: P,
+    set_style: oe,
+    space: G,
+    text: H,
+    toggle_class: B,
     transition_in: qe,
     transition_out: Te,
-    update_slot_base: In
+    update_slot_base: Yi
 } = window.__gradio__svelte__internal, {
-    tick: Wn
+    tick: Gi
 } = window.__gradio__svelte__internal, {
-    onDestroy: Un
-} = window.__gradio__svelte__internal, Xn = (l) => ({}), Tt = (l) => ({});
+    onDestroy: Ji
+} = window.__gradio__svelte__internal, Ki = (l) => ({}), Dt = (l) => ({});
 
-function Lt(l, e, t) {
+function Bt(l, e, t) {
     const n = l.slice();
     return n[38] = e[t], n[40] = t, n;
 }
 
-function St(l, e, t) {
+function Pt(l, e, t) {
     const n = l.slice();
     return n[38] = e[t], n;
 }
 
-function Yn(l) {
+function Qi(l) {
     let e, t = (
             /*i18n*/
             l[1]("common.error") + ""
         ),
-        n, i, s;
-    const o = (
+        n, i, o;
+    const s = (
             /*#slots*/
             l[29].error
         ),
-        r = En(
-            o,
+        f = Zi(
+            s,
             l,
             /*$$scope*/
             l[28],
-            Tt
+            Dt
         );
     return {
         c() {
-            e = $("span"), n = F(t), i = J(), r && r.c(), G(e, "class", "error svelte-1txqlrd");
+            e = $("span"), n = H(t), i = G(), f && f.c(), Y(e, "class", "error svelte-1txqlrd");
         },
-        m(a, f) {
-            v(a, e, f), re(e, n), v(a, i, f), r && r.m(a, f), s = !0;
+        m(a, _) {
+            p(a, e, _), ce(e, n), p(a, i, _), f && f.m(a, _), o = !0;
         },
-        p(a, f) {
-            (!s || f[0] & /*i18n*/
+        p(a, _) {
+            (!o || _[0] & /*i18n*/
                 2) && t !== (t = /*i18n*/
-                a[1]("common.error") + "") && O(n, t), r && r.p && (!s || f[0] & /*$$scope*/
-                268435456) && In(
-                r,
-                o,
+                a[1]("common.error") + "") && P(n, t), f && f.p && (!o || _[0] & /*$$scope*/
+                268435456) && Yi(
+                f,
+                s,
                 a,
                 /*$$scope*/
                 a[28],
-                s ? On(
-                    o,
+                o ? Wi(
+                    s,
                     /*$$scope*/
                     a[28],
-                    f,
-                    Xn
-                ) : Zn(
+                    _,
+                    Ki
+                ) : Ai(
                     /*$$scope*/
                     a[28]
                 ),
-                Tt
+                Dt
             );
         },
         i(a) {
-            s || (qe(r, a), s = !0);
+            o || (qe(f, a), o = !0);
         },
         o(a) {
-            Te(r, a), s = !1;
+            Te(f, a), o = !1;
         },
         d(a) {
-            a && (k(e), k(i)), r && r.d(a);
+            a && (v(e), v(i)), f && f.d(a);
         }
     };
 }
 
-function Gn(l) {
-    let e, t, n, i, s, o, r, a, f, _ = (
+function xi(l) {
+    let e, t, n, i, o, s, f, a, _, r = (
         /*variant*/
         l[8] === "default" && /*show_eta_bar*/
         l[18] && /*show_progress*/
-        l[6] === "full" && Ft(l)
+        l[6] === "full" && Zt(l)
     );
 
-    function u(d, p) {
+    function u(d, C) {
         if (
             /*progress*/
             d[7]
         )
-            return Qn;
+            return to;
         if (
             /*queue_position*/
             d[2] !== null && /*queue_size*/
             d[3] !== void 0 && /*queue_position*/
             d[2] >= 0
         )
-            return Kn;
+            return eo;
         if (
             /*queue_position*/
             d[2] === 0
         )
-            return Jn;
+            return $i;
     }
     let c = u(l),
         m = c && c(l),
-        y = (
+        k = (
             /*timer*/
-            l[5] && jt(l)
+            l[5] && Wt(l)
         );
-    const S = [ti, ei],
-        T = [];
+    const L = [oo, io],
+        S = [];
 
-    function L(d, p) {
+    function T(d, C) {
         return (
             /*last_progress_level*/
             d[15] != null ? 0 : (
                 /*show_progress*/
                 d[6] === "full" ? 1 : -1
             )
         );
     }
-    ~(s = L(l)) && (o = T[s] = S[s](l));
-    let C = ! /*timer*/
-        l[5] && Zt(l);
+    ~(o = T(l)) && (s = S[o] = L[o](l));
+    let y = ! /*timer*/
+        l[5] && Kt(l);
     return {
         c() {
-            _ && _.c(), e = J(), t = $("div"), m && m.c(), n = J(), y && y.c(), i = J(), o && o.c(), r = J(), C && C.c(), a = Le(), G(t, "class", "progress-text svelte-1txqlrd"), Z(
+            r && r.c(), e = G(), t = $("div"), m && m.c(), n = G(), k && k.c(), i = G(), s && s.c(), f = G(), y && y.c(), a = Se(), Y(t, "class", "progress-text svelte-1txqlrd"), B(
                 t,
                 "meta-text-center",
                 /*variant*/
                 l[8] === "center"
-            ), Z(
+            ), B(
                 t,
                 "meta-text",
                 /*variant*/
                 l[8] === "default"
             );
         },
-        m(d, p) {
-            _ && _.m(d, p), v(d, e, p), v(d, t, p), m && m.m(t, null), re(t, n), y && y.m(t, null), v(d, i, p), ~s && T[s].m(d, p), v(d, r, p), C && C.m(d, p), v(d, a, p), f = !0;
+        m(d, C) {
+            r && r.m(d, C), p(d, e, C), p(d, t, C), m && m.m(t, null), ce(t, n), k && k.m(t, null), p(d, i, C), ~o && S[o].m(d, C), p(d, f, C), y && y.m(d, C), p(d, a, C), _ = !0;
         },
-        p(d, p) {
+        p(d, C) {
             /*variant*/
             d[8] === "default" && /*show_eta_bar*/
                 d[18] && /*show_progress*/
-                d[6] === "full" ? _ ? _.p(d, p) : (_ = Ft(d), _.c(), _.m(e.parentNode, e)) : _ && (_.d(1), _ = null), c === (c = u(d)) && m ? m.p(d, p) : (m && m.d(1), m = c && c(d), m && (m.c(), m.m(t, n))), /*timer*/
-                d[5] ? y ? y.p(d, p) : (y = jt(d), y.c(), y.m(t, null)) : y && (y.d(1), y = null), (!f || p[0] & /*variant*/
-                    256) && Z(
+                d[6] === "full" ? r ? r.p(d, C) : (r = Zt(d), r.c(), r.m(e.parentNode, e)) : r && (r.d(1), r = null), c === (c = u(d)) && m ? m.p(d, C) : (m && m.d(1), m = c && c(d), m && (m.c(), m.m(t, n))), /*timer*/
+                d[5] ? k ? k.p(d, C) : (k = Wt(d), k.c(), k.m(t, null)) : k && (k.d(1), k = null), (!_ || C[0] & /*variant*/
+                    256) && B(
                     t,
                     "meta-text-center",
                     /*variant*/
                     d[8] === "center"
-                ), (!f || p[0] & /*variant*/
-                    256) && Z(
+                ), (!_ || C[0] & /*variant*/
+                    256) && B(
                     t,
                     "meta-text",
                     /*variant*/
                     d[8] === "default"
                 );
-            let H = s;
-            s = L(d), s === H ? ~s && T[s].p(d, p) : (o && ($t(), Te(T[H], 1, 1, () => {
-                    T[H] = null;
-                }), Qt()), ~s ? (o = T[s], o ? o.p(d, p) : (o = T[s] = S[s](d), o.c()), qe(o, 1), o.m(r.parentNode, r)) : o = null), /*timer*/
-                d[5] ? C && (C.d(1), C = null) : C ? C.p(d, p) : (C = Zt(d), C.c(), C.m(a.parentNode, a));
+            let j = o;
+            o = T(d), o === j ? ~o && S[o].p(d, C) : (s && (vl(), Te(S[j], 1, 1, () => {
+                    S[j] = null;
+                }), bl()), ~o ? (s = S[o], s ? s.p(d, C) : (s = S[o] = L[o](d), s.c()), qe(s, 1), s.m(f.parentNode, f)) : s = null), /*timer*/
+                d[5] ? y && (y.d(1), y = null) : y ? y.p(d, C) : (y = Kt(d), y.c(), y.m(a.parentNode, a));
         },
         i(d) {
-            f || (qe(o), f = !0);
+            _ || (qe(s), _ = !0);
         },
         o(d) {
-            Te(o), f = !1;
+            Te(s), _ = !1;
         },
         d(d) {
-            d && (k(e), k(t), k(i), k(r), k(a)), _ && _.d(d), m && m.d(), y && y.d(), ~s && T[s].d(d), C && C.d(d);
+            d && (v(e), v(t), v(i), v(f), v(a)), r && r.d(d), m && m.d(), k && k.d(), ~o && S[o].d(d), y && y.d(d);
         }
     };
 }
 
-function Ft(l) {
+function Zt(l) {
     let e, t = `translateX(${/*eta_level*/
   (l[17] || 0) * 100 - 100}%)`;
     return {
         c() {
-            e = $("div"), G(e, "class", "eta-bar svelte-1txqlrd"), se(e, "transform", t);
+            e = $("div"), Y(e, "class", "eta-bar svelte-1txqlrd"), oe(e, "transform", t);
         },
         m(n, i) {
-            v(n, e, i);
+            p(n, e, i);
         },
         p(n, i) {
             i[0] & /*eta_level*/
                 131072 && t !== (t = `translateX(${/*eta_level*/
-      (n[17] || 0) * 100 - 100}%)`) && se(e, "transform", t);
+      (n[17] || 0) * 100 - 100}%)`) && oe(e, "transform", t);
         },
         d(n) {
-            n && k(e);
+            n && v(e);
         }
     };
 }
 
-function Jn(l) {
+function $i(l) {
     let e;
     return {
         c() {
-            e = F("processing |");
+            e = H("processing |");
         },
         m(t, n) {
-            v(t, e, n);
+            p(t, e, n);
         },
-        p: Ue,
+        p: Ge,
         d(t) {
-            t && k(e);
+            t && v(e);
         }
     };
 }
 
-function Kn(l) {
+function eo(l) {
     let e, t = (
             /*queue_position*/
             l[2] + 1 + ""
         ),
-        n, i, s, o;
+        n, i, o, s;
     return {
         c() {
-            e = F("queue: "), n = F(t), i = F("/"), s = F(
+            e = H("queue: "), n = H(t), i = H("/"), o = H(
                 /*queue_size*/
                 l[3]
-            ), o = F(" |");
+            ), s = H(" |");
         },
-        m(r, a) {
-            v(r, e, a), v(r, n, a), v(r, i, a), v(r, s, a), v(r, o, a);
+        m(f, a) {
+            p(f, e, a), p(f, n, a), p(f, i, a), p(f, o, a), p(f, s, a);
         },
-        p(r, a) {
+        p(f, a) {
             a[0] & /*queue_position*/
                 4 && t !== (t = /*queue_position*/
-                    r[2] + 1 + "") && O(n, t), a[0] & /*queue_size*/
-                8 && O(
-                    s,
+                    f[2] + 1 + "") && P(n, t), a[0] & /*queue_size*/
+                8 && P(
+                    o,
                     /*queue_size*/
-                    r[3]
+                    f[3]
                 );
         },
-        d(r) {
-            r && (k(e), k(n), k(i), k(s), k(o));
+        d(f) {
+            f && (v(e), v(n), v(i), v(o), v(s));
         }
     };
 }
 
-function Qn(l) {
-    let e, t = Pe(
+function to(l) {
+    let e, t = Be(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let i = 0; i < t.length; i += 1)
-        n[i] = Mt(St(l, t, i));
+        n[i] = At(Pt(l, t, i));
     return {
         c() {
             for (let i = 0; i < n.length; i += 1)
                 n[i].c();
-            e = Le();
+            e = Se();
         },
-        m(i, s) {
-            for (let o = 0; o < n.length; o += 1)
-                n[o] && n[o].m(i, s);
-            v(i, e, s);
+        m(i, o) {
+            for (let s = 0; s < n.length; s += 1)
+                n[s] && n[s].m(i, o);
+            p(i, e, o);
         },
-        p(i, s) {
-            if (s[0] & /*progress*/
+        p(i, o) {
+            if (o[0] & /*progress*/
                 128) {
-                t = Pe(
+                t = Be(
                     /*progress*/
                     i[7]
                 );
-                let o;
-                for (o = 0; o < t.length; o += 1) {
-                    const r = St(i, t, o);
-                    n[o] ? n[o].p(r, s) : (n[o] = Mt(r), n[o].c(), n[o].m(e.parentNode, e));
+                let s;
+                for (s = 0; s < t.length; s += 1) {
+                    const f = Pt(i, t, s);
+                    n[s] ? n[s].p(f, o) : (n[s] = At(f), n[s].c(), n[s].m(e.parentNode, e));
                 }
-                for (; o < n.length; o += 1)
-                    n[o].d(1);
+                for (; s < n.length; s += 1)
+                    n[s].d(1);
                 n.length = t.length;
             }
         },
         d(i) {
-            i && k(e), xt(n, i);
+            i && v(e), wl(n, i);
         }
     };
 }
 
-function Ht(l) {
+function Ot(l) {
     let e, t = (
             /*p*/
             l[38].unit + ""
         ),
-        n, i, s = " ",
-        o;
+        n, i, o = " ",
+        s;
 
-    function r(_, u) {
+    function f(r, u) {
         return (
             /*p*/
-            _[38].length != null ? $n : xn
+            r[38].length != null ? no : lo
         );
     }
-    let a = r(l),
-        f = a(l);
+    let a = f(l),
+        _ = a(l);
     return {
         c() {
-            f.c(), e = J(), n = F(t), i = F(" | "), o = F(s);
+            _.c(), e = G(), n = H(t), i = H(" | "), s = H(o);
         },
-        m(_, u) {
-            f.m(_, u), v(_, e, u), v(_, n, u), v(_, i, u), v(_, o, u);
+        m(r, u) {
+            _.m(r, u), p(r, e, u), p(r, n, u), p(r, i, u), p(r, s, u);
         },
-        p(_, u) {
-            a === (a = r(_)) && f ? f.p(_, u) : (f.d(1), f = a(_), f && (f.c(), f.m(e.parentNode, e))), u[0] & /*progress*/
+        p(r, u) {
+            a === (a = f(r)) && _ ? _.p(r, u) : (_.d(1), _ = a(r), _ && (_.c(), _.m(e.parentNode, e))), u[0] & /*progress*/
                 128 && t !== (t = /*p*/
-                    _[38].unit + "") && O(n, t);
+                    r[38].unit + "") && P(n, t);
         },
-        d(_) {
-            _ && (k(e), k(n), k(i), k(o)), f.d(_);
+        d(r) {
+            r && (v(e), v(n), v(i), v(s)), _.d(r);
         }
     };
 }
 
-function xn(l) {
-    let e = pe(
+function lo(l) {
+    let e = ke(
             /*p*/
             l[38].index || 0
         ) + "",
         t;
     return {
         c() {
-            t = F(e);
+            t = H(e);
         },
         m(n, i) {
-            v(n, t, i);
+            p(n, t, i);
         },
         p(n, i) {
             i[0] & /*progress*/
-                128 && e !== (e = pe(
+                128 && e !== (e = ke(
                     /*p*/
                     n[38].index || 0
-                ) + "") && O(t, e);
+                ) + "") && P(t, e);
         },
         d(n) {
-            n && k(t);
+            n && v(t);
         }
     };
 }
 
-function $n(l) {
-    let e = pe(
+function no(l) {
+    let e = ke(
             /*p*/
             l[38].index || 0
         ) + "",
-        t, n, i = pe(
+        t, n, i = ke(
             /*p*/
             l[38].length
         ) + "",
-        s;
+        o;
     return {
         c() {
-            t = F(e), n = F("/"), s = F(i);
+            t = H(e), n = H("/"), o = H(i);
         },
-        m(o, r) {
-            v(o, t, r), v(o, n, r), v(o, s, r);
+        m(s, f) {
+            p(s, t, f), p(s, n, f), p(s, o, f);
         },
-        p(o, r) {
-            r[0] & /*progress*/
-                128 && e !== (e = pe(
+        p(s, f) {
+            f[0] & /*progress*/
+                128 && e !== (e = ke(
                     /*p*/
-                    o[38].index || 0
-                ) + "") && O(t, e), r[0] & /*progress*/
-                128 && i !== (i = pe(
+                    s[38].index || 0
+                ) + "") && P(t, e), f[0] & /*progress*/
+                128 && i !== (i = ke(
                     /*p*/
-                    o[38].length
-                ) + "") && O(s, i);
+                    s[38].length
+                ) + "") && P(o, i);
         },
-        d(o) {
-            o && (k(t), k(n), k(s));
+        d(s) {
+            s && (v(t), v(n), v(o));
         }
     };
 }
 
-function Mt(l) {
+function At(l) {
     let e, t = (
         /*p*/
-        l[38].index != null && Ht(l)
+        l[38].index != null && Ot(l)
     );
     return {
         c() {
-            t && t.c(), e = Le();
+            t && t.c(), e = Se();
         },
         m(n, i) {
-            t && t.m(n, i), v(n, e, i);
+            t && t.m(n, i), p(n, e, i);
         },
         p(n, i) {
             /*p*/
-            n[38].index != null ? t ? t.p(n, i) : (t = Ht(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+            n[38].index != null ? t ? t.p(n, i) : (t = Ot(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && k(e), t && t.d(n);
+            n && v(e), t && t.d(n);
         }
     };
 }
 
-function jt(l) {
+function Wt(l) {
     let e, t = (
             /*eta*/
             l[0] ? `/${/*formatted_eta*/
     l[19]}` : ""
         ),
         n, i;
     return {
         c() {
-            e = F(
+            e = H(
                 /*formatted_timer*/
                 l[20]
-            ), n = F(t), i = F("s");
+            ), n = H(t), i = H("s");
         },
-        m(s, o) {
-            v(s, e, o), v(s, n, o), v(s, i, o);
+        m(o, s) {
+            p(o, e, s), p(o, n, s), p(o, i, s);
         },
-        p(s, o) {
-            o[0] & /*formatted_timer*/
-                1048576 && O(
+        p(o, s) {
+            s[0] & /*formatted_timer*/
+                1048576 && P(
                     e,
                     /*formatted_timer*/
-                    s[20]
-                ), o[0] & /*eta, formatted_eta*/
+                    o[20]
+                ), s[0] & /*eta, formatted_eta*/
                 524289 && t !== (t = /*eta*/
-                    s[0] ? `/${/*formatted_eta*/
-      s[19]}` : "") && O(n, t);
+                    o[0] ? `/${/*formatted_eta*/
+      o[19]}` : "") && P(n, t);
         },
-        d(s) {
-            s && (k(e), k(n), k(i));
+        d(o) {
+            o && (v(e), v(n), v(i));
         }
     };
 }
 
-function ei(l) {
+function io(l) {
     let e, t;
-    return e = new Vn({
+    return e = new Di({
         props: {
             margin: (
                 /*variant*/
                 l[8] === "default"
             )
         }
     }), {
         c() {
-            Bn(e.$$.fragment);
+            Pi(e.$$.fragment);
         },
         m(n, i) {
-            An(e, n, i), t = !0;
+            Ui(e, n, i), t = !0;
         },
         p(n, i) {
-            const s = {};
+            const o = {};
             i[0] & /*variant*/
-                256 && (s.margin = /*variant*/
-                    n[8] === "default"), e.$set(s);
+                256 && (o.margin = /*variant*/
+                    n[8] === "default"), e.$set(o);
         },
         i(n) {
             t || (qe(e.$$.fragment, n), t = !0);
         },
         o(n) {
             Te(e.$$.fragment, n), t = !1;
         },
         d(n) {
-            Pn(e, n);
+            Oi(e, n);
         }
     };
 }
 
-function ti(l) {
-    let e, t, n, i, s, o = `${/*last_progress_level*/
+function oo(l) {
+    let e, t, n, i, o, s = `${/*last_progress_level*/
   l[15] * 100}%`,
-        r = (
+        f = (
             /*progress*/
-            l[7] != null && Nt(l)
+            l[7] != null && It(l)
         );
     return {
         c() {
-            e = $("div"), t = $("div"), r && r.c(), n = J(), i = $("div"), s = $("div"), G(t, "class", "progress-level-inner svelte-1txqlrd"), G(s, "class", "progress-bar svelte-1txqlrd"), se(s, "width", o), G(i, "class", "progress-bar-wrap svelte-1txqlrd"), G(e, "class", "progress-level svelte-1txqlrd");
+            e = $("div"), t = $("div"), f && f.c(), n = G(), i = $("div"), o = $("div"), Y(t, "class", "progress-level-inner svelte-1txqlrd"), Y(o, "class", "progress-bar svelte-1txqlrd"), oe(o, "width", s), Y(i, "class", "progress-bar-wrap svelte-1txqlrd"), Y(e, "class", "progress-level svelte-1txqlrd");
         },
-        m(a, f) {
-            v(a, e, f), re(e, t), r && r.m(t, null), re(e, n), re(e, i), re(i, s), l[30](s);
+        m(a, _) {
+            p(a, e, _), ce(e, t), f && f.m(t, null), ce(e, n), ce(e, i), ce(i, o), l[30](o);
         },
-        p(a, f) {
+        p(a, _) {
             /*progress*/
-            a[7] != null ? r ? r.p(a, f) : (r = Nt(a), r.c(), r.m(t, null)) : r && (r.d(1), r = null), f[0] & /*last_progress_level*/
-                32768 && o !== (o = `${/*last_progress_level*/
-      a[15] * 100}%`) && se(s, "width", o);
+            a[7] != null ? f ? f.p(a, _) : (f = It(a), f.c(), f.m(t, null)) : f && (f.d(1), f = null), _[0] & /*last_progress_level*/
+                32768 && s !== (s = `${/*last_progress_level*/
+      a[15] * 100}%`) && oe(o, "width", s);
         },
-        i: Ue,
-        o: Ue,
+        i: Ge,
+        o: Ge,
         d(a) {
-            a && k(e), r && r.d(), l[30](null);
+            a && v(e), f && f.d(), l[30](null);
         }
     };
 }
 
-function Nt(l) {
-    let e, t = Pe(
+function It(l) {
+    let e, t = Be(
             /*progress*/
             l[7]
         ),
         n = [];
     for (let i = 0; i < t.length; i += 1)
-        n[i] = Pt(Lt(l, t, i));
+        n[i] = Jt(Bt(l, t, i));
     return {
         c() {
             for (let i = 0; i < n.length; i += 1)
                 n[i].c();
-            e = Le();
+            e = Se();
         },
-        m(i, s) {
-            for (let o = 0; o < n.length; o += 1)
-                n[o] && n[o].m(i, s);
-            v(i, e, s);
+        m(i, o) {
+            for (let s = 0; s < n.length; s += 1)
+                n[s] && n[s].m(i, o);
+            p(i, e, o);
         },
-        p(i, s) {
-            if (s[0] & /*progress_level, progress*/
+        p(i, o) {
+            if (o[0] & /*progress_level, progress*/
                 16512) {
-                t = Pe(
+                t = Be(
                     /*progress*/
                     i[7]
                 );
-                let o;
-                for (o = 0; o < t.length; o += 1) {
-                    const r = Lt(i, t, o);
-                    n[o] ? n[o].p(r, s) : (n[o] = Pt(r), n[o].c(), n[o].m(e.parentNode, e));
+                let s;
+                for (s = 0; s < t.length; s += 1) {
+                    const f = Bt(i, t, s);
+                    n[s] ? n[s].p(f, o) : (n[s] = Jt(f), n[s].c(), n[s].m(e.parentNode, e));
                 }
-                for (; o < n.length; o += 1)
-                    n[o].d(1);
+                for (; s < n.length; s += 1)
+                    n[s].d(1);
                 n.length = t.length;
             }
         },
         d(i) {
-            i && k(e), xt(n, i);
+            i && v(e), wl(n, i);
         }
     };
 }
 
-function Vt(l) {
-    let e, t, n, i, s = (
+function Ut(l) {
+    let e, t, n, i, o = (
             /*i*/
-            l[40] !== 0 && li()
+            l[40] !== 0 && so()
         ),
-        o = (
+        s = (
             /*p*/
-            l[38].desc != null && zt(l)
+            l[38].desc != null && Xt(l)
         ),
-        r = (
+        f = (
             /*p*/
             l[38].desc != null && /*progress_level*/
             l[14] && /*progress_level*/
             l[14][
                 /*i*/
                 l[40]
-            ] != null && Bt()
+            ] != null && Yt()
         ),
         a = (
             /*progress_level*/
-            l[14] != null && Et(l)
+            l[14] != null && Gt(l)
         );
     return {
         c() {
-            s && s.c(), e = J(), o && o.c(), t = J(), r && r.c(), n = J(), a && a.c(), i = Le();
+            o && o.c(), e = G(), s && s.c(), t = G(), f && f.c(), n = G(), a && a.c(), i = Se();
         },
-        m(f, _) {
-            s && s.m(f, _), v(f, e, _), o && o.m(f, _), v(f, t, _), r && r.m(f, _), v(f, n, _), a && a.m(f, _), v(f, i, _);
+        m(_, r) {
+            o && o.m(_, r), p(_, e, r), s && s.m(_, r), p(_, t, r), f && f.m(_, r), p(_, n, r), a && a.m(_, r), p(_, i, r);
         },
-        p(f, _) {
+        p(_, r) {
             /*p*/
-            f[38].desc != null ? o ? o.p(f, _) : (o = zt(f), o.c(), o.m(t.parentNode, t)) : o && (o.d(1), o = null), /*p*/
-                f[38].desc != null && /*progress_level*/
-                f[14] && /*progress_level*/
-                f[14][
+            _[38].desc != null ? s ? s.p(_, r) : (s = Xt(_), s.c(), s.m(t.parentNode, t)) : s && (s.d(1), s = null), /*p*/
+                _[38].desc != null && /*progress_level*/
+                _[14] && /*progress_level*/
+                _[14][
                     /*i*/
-                    f[40]
-                ] != null ? r || (r = Bt(), r.c(), r.m(n.parentNode, n)) : r && (r.d(1), r = null), /*progress_level*/
-                f[14] != null ? a ? a.p(f, _) : (a = Et(f), a.c(), a.m(i.parentNode, i)) : a && (a.d(1), a = null);
+                    _[40]
+                ] != null ? f || (f = Yt(), f.c(), f.m(n.parentNode, n)) : f && (f.d(1), f = null), /*progress_level*/
+                _[14] != null ? a ? a.p(_, r) : (a = Gt(_), a.c(), a.m(i.parentNode, i)) : a && (a.d(1), a = null);
         },
-        d(f) {
-            f && (k(e), k(t), k(n), k(i)), s && s.d(f), o && o.d(f), r && r.d(f), a && a.d(f);
+        d(_) {
+            _ && (v(e), v(t), v(n), v(i)), o && o.d(_), s && s.d(_), f && f.d(_), a && a.d(_);
         }
     };
 }
 
-function li(l) {
+function so(l) {
     let e;
     return {
         c() {
-            e = F(" /");
+            e = H(" /");
         },
         m(t, n) {
-            v(t, e, n);
+            p(t, e, n);
         },
         d(t) {
-            t && k(e);
+            t && v(e);
         }
     };
 }
 
-function zt(l) {
+function Xt(l) {
     let e = (
             /*p*/
             l[38].desc + ""
         ),
         t;
     return {
         c() {
-            t = F(e);
+            t = H(e);
         },
         m(n, i) {
-            v(n, t, i);
+            p(n, t, i);
         },
         p(n, i) {
             i[0] & /*progress*/
                 128 && e !== (e = /*p*/
-                    n[38].desc + "") && O(t, e);
+                    n[38].desc + "") && P(t, e);
         },
         d(n) {
-            n && k(t);
+            n && v(t);
         }
     };
 }
 
-function Bt(l) {
+function Yt(l) {
     let e;
     return {
         c() {
-            e = F("-");
+            e = H("-");
         },
         m(t, n) {
-            v(t, e, n);
+            p(t, e, n);
         },
         d(t) {
-            t && k(e);
+            t && v(e);
         }
     };
 }
 
-function Et(l) {
+function Gt(l) {
     let e = (100 * /*progress_level*/
             (l[14][
                 /*i*/
                 l[40]
             ] || 0)).toFixed(1) + "",
         t, n;
     return {
         c() {
-            t = F(e), n = F("%");
+            t = H(e), n = H("%");
         },
-        m(i, s) {
-            v(i, t, s), v(i, n, s);
+        m(i, o) {
+            p(i, t, o), p(i, n, o);
         },
-        p(i, s) {
-            s[0] & /*progress_level*/
+        p(i, o) {
+            o[0] & /*progress_level*/
                 16384 && e !== (e = (100 * /*progress_level*/
                     (i[14][
                         /*i*/
                         i[40]
-                    ] || 0)).toFixed(1) + "") && O(t, e);
+                    ] || 0)).toFixed(1) + "") && P(t, e);
         },
         d(i) {
-            i && (k(t), k(n));
+            i && (v(t), v(n));
         }
     };
 }
 
-function Pt(l) {
+function Jt(l) {
     let e, t = (
         /*p*/
         (l[38].desc != null || /*progress_level*/
             l[14] && /*progress_level*/
             l[14][
                 /*i*/
                 l[40]
-            ] != null) && Vt(l)
+            ] != null) && Ut(l)
     );
     return {
         c() {
-            t && t.c(), e = Le();
+            t && t.c(), e = Se();
         },
         m(n, i) {
-            t && t.m(n, i), v(n, e, i);
+            t && t.m(n, i), p(n, e, i);
         },
         p(n, i) {
             /*p*/
             n[38].desc != null || /*progress_level*/
                 n[14] && /*progress_level*/
                 n[14][
                     /*i*/
                     n[40]
-                ] != null ? t ? t.p(n, i) : (t = Vt(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
+                ] != null ? t ? t.p(n, i) : (t = Ut(n), t.c(), t.m(e.parentNode, e)) : t && (t.d(1), t = null);
         },
         d(n) {
-            n && k(e), t && t.d(n);
+            n && v(e), t && t.d(n);
         }
     };
 }
 
-function Zt(l) {
+function Kt(l) {
     let e, t;
     return {
         c() {
-            e = $("p"), t = F(
+            e = $("p"), t = H(
                 /*loading_text*/
                 l[9]
-            ), G(e, "class", "loading svelte-1txqlrd");
+            ), Y(e, "class", "loading svelte-1txqlrd");
         },
         m(n, i) {
-            v(n, e, i), re(e, t);
+            p(n, e, i), ce(e, t);
         },
         p(n, i) {
             i[0] & /*loading_text*/
-                512 && O(
+                512 && P(
                     t,
                     /*loading_text*/
                     n[9]
                 );
         },
         d(n) {
-            n && k(e);
+            n && v(e);
         }
     };
 }
 
-function ni(l) {
-    let e, t, n, i, s;
-    const o = [Gn, Yn],
-        r = [];
+function fo(l) {
+    let e, t, n, i, o;
+    const s = [xi, Qi],
+        f = [];
 
-    function a(f, _) {
+    function a(_, r) {
         return (
             /*status*/
-            f[4] === "pending" ? 0 : (
+            _[4] === "pending" ? 0 : (
                 /*status*/
-                f[4] === "error" ? 1 : -1
+                _[4] === "error" ? 1 : -1
             )
         );
     }
-    return ~(t = a(l)) && (n = r[t] = o[t](l)), {
+    return ~(t = a(l)) && (n = f[t] = s[t](l)), {
         c() {
-            e = $("div"), n && n.c(), G(e, "class", i = "wrap " + /*variant*/
+            e = $("div"), n && n.c(), Y(e, "class", i = "wrap " + /*variant*/
                 l[8] + " " + /*show_progress*/
-                l[6] + " svelte-1txqlrd"), Z(e, "hide", ! /*status*/
+                l[6] + " svelte-1txqlrd"), B(e, "hide", ! /*status*/
                 l[4] || /*status*/
                 l[4] === "complete" || /*show_progress*/
-                l[6] === "hidden"), Z(
+                l[6] === "hidden"), B(
                 e,
                 "translucent",
                 /*variant*/
                 l[8] === "center" && /*status*/
                 (l[4] === "pending" || /*status*/
                     l[4] === "error") || /*translucent*/
                 l[11] || /*show_progress*/
                 l[6] === "minimal"
-            ), Z(
+            ), B(
                 e,
                 "generating",
                 /*status*/
                 l[4] === "generating"
-            ), Z(
+            ), B(
                 e,
                 "border",
                 /*border*/
                 l[12]
-            ), se(
+            ), oe(
                 e,
                 "position",
                 /*absolute*/
                 l[10] ? "absolute" : "static"
-            ), se(
+            ), oe(
                 e,
                 "padding",
                 /*absolute*/
                 l[10] ? "0" : "var(--size-8) 0"
             );
         },
-        m(f, _) {
-            v(f, e, _), ~t && r[t].m(e, null), l[31](e), s = !0;
+        m(_, r) {
+            p(_, e, r), ~t && f[t].m(e, null), l[31](e), o = !0;
         },
-        p(f, _) {
+        p(_, r) {
             let u = t;
-            t = a(f), t === u ? ~t && r[t].p(f, _) : (n && ($t(), Te(r[u], 1, 1, () => {
-                    r[u] = null;
-                }), Qt()), ~t ? (n = r[t], n ? n.p(f, _) : (n = r[t] = o[t](f), n.c()), qe(n, 1), n.m(e, null)) : n = null), (!s || _[0] & /*variant, show_progress*/
+            t = a(_), t === u ? ~t && f[t].p(_, r) : (n && (vl(), Te(f[u], 1, 1, () => {
+                    f[u] = null;
+                }), bl()), ~t ? (n = f[t], n ? n.p(_, r) : (n = f[t] = s[t](_), n.c()), qe(n, 1), n.m(e, null)) : n = null), (!o || r[0] & /*variant, show_progress*/
                     320 && i !== (i = "wrap " + /*variant*/
-                        f[8] + " " + /*show_progress*/
-                        f[6] + " svelte-1txqlrd")) && G(e, "class", i), (!s || _[0] & /*variant, show_progress, status, show_progress*/
-                    336) && Z(e, "hide", ! /*status*/
-                    f[4] || /*status*/
-                    f[4] === "complete" || /*show_progress*/
-                    f[6] === "hidden"), (!s || _[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
-                    2384) && Z(
+                        _[8] + " " + /*show_progress*/
+                        _[6] + " svelte-1txqlrd")) && Y(e, "class", i), (!o || r[0] & /*variant, show_progress, status, show_progress*/
+                    336) && B(e, "hide", ! /*status*/
+                    _[4] || /*status*/
+                    _[4] === "complete" || /*show_progress*/
+                    _[6] === "hidden"), (!o || r[0] & /*variant, show_progress, variant, status, translucent, show_progress*/
+                    2384) && B(
                     e,
                     "translucent",
                     /*variant*/
-                    f[8] === "center" && /*status*/
-                    (f[4] === "pending" || /*status*/
-                        f[4] === "error") || /*translucent*/
-                    f[11] || /*show_progress*/
-                    f[6] === "minimal"
-                ), (!s || _[0] & /*variant, show_progress, status*/
-                    336) && Z(
+                    _[8] === "center" && /*status*/
+                    (_[4] === "pending" || /*status*/
+                        _[4] === "error") || /*translucent*/
+                    _[11] || /*show_progress*/
+                    _[6] === "minimal"
+                ), (!o || r[0] & /*variant, show_progress, status*/
+                    336) && B(
                     e,
                     "generating",
                     /*status*/
-                    f[4] === "generating"
-                ), (!s || _[0] & /*variant, show_progress, border*/
-                    4416) && Z(
+                    _[4] === "generating"
+                ), (!o || r[0] & /*variant, show_progress, border*/
+                    4416) && B(
                     e,
                     "border",
                     /*border*/
-                    f[12]
-                ), _[0] & /*absolute*/
-                1024 && se(
+                    _[12]
+                ), r[0] & /*absolute*/
+                1024 && oe(
                     e,
                     "position",
                     /*absolute*/
-                    f[10] ? "absolute" : "static"
-                ), _[0] & /*absolute*/
-                1024 && se(
+                    _[10] ? "absolute" : "static"
+                ), r[0] & /*absolute*/
+                1024 && oe(
                     e,
                     "padding",
                     /*absolute*/
-                    f[10] ? "0" : "var(--size-8) 0"
+                    _[10] ? "0" : "var(--size-8) 0"
                 );
         },
-        i(f) {
-            s || (qe(n), s = !0);
+        i(_) {
+            o || (qe(n), o = !0);
         },
-        o(f) {
-            Te(n), s = !1;
+        o(_) {
+            Te(n), o = !1;
         },
-        d(f) {
-            f && k(e), ~t && r[t].d(), l[31](null);
+        d(_) {
+            _ && v(e), ~t && f[t].d(), l[31](null);
         }
     };
 }
-let Be = [],
-    Ie = !1;
-async function ii(l, e = !0) {
+let Ee = [],
+    Xe = !1;
+async function _o(l, e = !0) {
     if (!(window.__gradio_mode__ === "website" || window.__gradio_mode__ !== "app" && e !== !0)) {
-        if (Be.push(l), !Ie)
-            Ie = !0;
+        if (Ee.push(l), !Xe)
+            Xe = !0;
         else
             return;
-        await Wn(), requestAnimationFrame(() => {
+        await Gi(), requestAnimationFrame(() => {
             let t = [0, 0];
-            for (let n = 0; n < Be.length; n++) {
-                const s = Be[n].getBoundingClientRect();
-                (n === 0 || s.top + window.scrollY <= t[0]) && (t[0] = s.top + window.scrollY, t[1] = n);
+            for (let n = 0; n < Ee.length; n++) {
+                const o = Ee[n].getBoundingClientRect();
+                (n === 0 || o.top + window.scrollY <= t[0]) && (t[0] = o.top + window.scrollY, t[1] = n);
             }
             window.scrollTo({
                 top: t[0] - 20,
                 behavior: "smooth"
-            }), Ie = !1, Be = [];
+            }), Xe = !1, Ee = [];
         });
     }
 }
 
-function si(l, e, t) {
+function ao(l, e, t) {
     let n, {
             $$slots: i = {},
-            $$scope: s
+            $$scope: o
         } = e,
         {
-            i18n: o
+            i18n: s
         } = e,
         {
-            eta: r = null
+            eta: f = null
         } = e,
         {
             queue_position: a
         } = e,
         {
-            queue_size: f
+            queue_size: _
         } = e,
         {
-            status: _
+            status: r
         } = e,
         {
             scroll_to_output: u = !1
         } = e,
         {
             timer: c = !0
         } = e,
         {
             show_progress: m = "full"
         } = e,
         {
-            message: y = null
+            message: k = null
         } = e,
         {
-            progress: S = null
+            progress: L = null
         } = e,
         {
-            variant: T = "default"
+            variant: S = "default"
         } = e,
         {
-            loading_text: L = "Loading..."
+            loading_text: T = "Loading..."
         } = e,
         {
-            absolute: C = !0
+            absolute: y = !0
         } = e,
         {
             translucent: d = !1
         } = e,
         {
-            border: p = !1
+            border: C = !1
         } = e,
         {
-            autoscroll: H
+            autoscroll: j
         } = e,
-        b, R = !1,
-        K = 0,
+        h, Z = !1,
+        J = 0,
         E = 0,
+        O = null,
+        R = null,
+        ae = 0,
         A = null,
-        X = null,
-        he = 0,
-        D = null,
-        Q, P = null,
-        be = !0;
-    const g = () => {
-        t(0, r = t(26, A = t(19, ge = null))), t(24, K = performance.now()), t(25, E = 0), R = !0, je();
+        K, D = null,
+        me = !0;
+    const Le = () => {
+        t(0, f = t(26, O = t(19, he = null))), t(24, J = performance.now()), t(25, E = 0), Z = !0, ge();
     };
 
-    function je() {
+    function ge() {
         requestAnimationFrame(() => {
-            t(25, E = (performance.now() - K) / 1e3), R && je();
+            t(25, E = (performance.now() - J) / 1e3), Z && ge();
         });
     }
 
-    function Ne() {
-        t(25, E = 0), t(0, r = t(26, A = t(19, ge = null))), R && (R = !1);
+    function b() {
+        t(25, E = 0), t(0, f = t(26, O = t(19, he = null))), Z && (Z = !1);
     }
-    Un(() => {
-        R && Ne();
+    Ji(() => {
+        Z && b();
     });
-    let ge = null;
+    let he = null;
 
-    function Ze(w) {
-        qt[w ? "unshift" : "push"](() => {
-            P = w, t(16, P), t(7, S), t(14, D), t(15, Q);
+    function Oe(w) {
+        Rt[w ? "unshift" : "push"](() => {
+            D = w, t(16, D), t(7, L), t(14, A), t(15, K);
         });
     }
 
-    function Oe(w) {
-        qt[w ? "unshift" : "push"](() => {
-            b = w, t(13, b);
+    function Ae(w) {
+        Rt[w ? "unshift" : "push"](() => {
+            h = w, t(13, h);
         });
     }
     return l.$$set = (w) => {
-        "i18n" in w && t(1, o = w.i18n), "eta" in w && t(0, r = w.eta), "queue_position" in w && t(2, a = w.queue_position), "queue_size" in w && t(3, f = w.queue_size), "status" in w && t(4, _ = w.status), "scroll_to_output" in w && t(21, u = w.scroll_to_output), "timer" in w && t(5, c = w.timer), "show_progress" in w && t(6, m = w.show_progress), "message" in w && t(22, y = w.message), "progress" in w && t(7, S = w.progress), "variant" in w && t(8, T = w.variant), "loading_text" in w && t(9, L = w.loading_text), "absolute" in w && t(10, C = w.absolute), "translucent" in w && t(11, d = w.translucent), "border" in w && t(12, p = w.border), "autoscroll" in w && t(23, H = w.autoscroll), "$$scope" in w && t(28, s = w.$$scope);
+        "i18n" in w && t(1, s = w.i18n), "eta" in w && t(0, f = w.eta), "queue_position" in w && t(2, a = w.queue_position), "queue_size" in w && t(3, _ = w.queue_size), "status" in w && t(4, r = w.status), "scroll_to_output" in w && t(21, u = w.scroll_to_output), "timer" in w && t(5, c = w.timer), "show_progress" in w && t(6, m = w.show_progress), "message" in w && t(22, k = w.message), "progress" in w && t(7, L = w.progress), "variant" in w && t(8, S = w.variant), "loading_text" in w && t(9, T = w.loading_text), "absolute" in w && t(10, y = w.absolute), "translucent" in w && t(11, d = w.translucent), "border" in w && t(12, C = w.border), "autoscroll" in w && t(23, j = w.autoscroll), "$$scope" in w && t(28, o = w.$$scope);
     }, l.$$.update = () => {
         l.$$.dirty[0] & /*eta, old_eta, timer_start, eta_from_start*/
-            218103809 && (r === null && t(0, r = A), r != null && A !== r && (t(27, X = (performance.now() - K) / 1e3 + r), t(19, ge = X.toFixed(1)), t(26, A = r))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
-            167772160 && t(17, he = X === null || X <= 0 || !E ? null : Math.min(E / X, 1)), l.$$.dirty[0] & /*progress*/
-            128 && S != null && t(18, be = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
-            114816 && (S != null ? t(14, D = S.map((w) => {
+            218103809 && (f === null && t(0, f = O), f != null && O !== f && (t(27, R = (performance.now() - J) / 1e3 + f), t(19, he = R.toFixed(1)), t(26, O = f))), l.$$.dirty[0] & /*eta_from_start, timer_diff*/
+            167772160 && t(17, ae = R === null || R <= 0 || !E ? null : Math.min(E / R, 1)), l.$$.dirty[0] & /*progress*/
+            128 && L != null && t(18, me = !1), l.$$.dirty[0] & /*progress, progress_level, progress_bar, last_progress_level*/
+            114816 && (L != null ? t(14, A = L.map((w) => {
                 if (w.index != null && w.length != null)
                     return w.index / w.length;
                 if (w.progress != null)
                     return w.progress;
-            })) : t(14, D = null), D ? (t(15, Q = D[D.length - 1]), P && (Q === 0 ? t(16, P.style.transition = "0", P) : t(16, P.style.transition = "150ms", P))) : t(15, Q = void 0)), l.$$.dirty[0] & /*status*/
-            16 && (_ === "pending" ? g() : Ne()), l.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
-            10493968 && b && u && (_ === "pending" || _ === "complete") && ii(b, H), l.$$.dirty[0] & /*status, message*/
+            })) : t(14, A = null), A ? (t(15, K = A[A.length - 1]), D && (K === 0 ? t(16, D.style.transition = "0", D) : t(16, D.style.transition = "150ms", D))) : t(15, K = void 0)), l.$$.dirty[0] & /*status*/
+            16 && (r === "pending" ? Le() : b()), l.$$.dirty[0] & /*el, scroll_to_output, status, autoscroll*/
+            10493968 && h && u && (r === "pending" || r === "complete") && _o(h, j), l.$$.dirty[0] & /*status, message*/
             4194320, l.$$.dirty[0] & /*timer_diff*/
             33554432 && t(20, n = E.toFixed(1));
     }, [
-        r,
-        o,
-        a,
         f,
+        s,
+        a,
         _,
+        r,
         c,
         m,
+        L,
         S,
         T,
-        L,
-        C,
+        y,
         d,
-        p,
-        b,
+        C,
+        h,
+        A,
+        K,
         D,
-        Q,
-        P,
+        ae,
+        me,
         he,
-        be,
-        ge,
         n,
         u,
-        y,
-        H,
-        K,
+        k,
+        j,
+        J,
         E,
-        A,
-        X,
-        s,
+        O,
+        R,
+        o,
         i,
-        Ze,
-        Oe
+        Oe,
+        Ae
     ];
 }
-class oi extends zn {
+class ro extends Bi {
     constructor(e) {
-        super(), Rn(
+        super(), Ii(
             this,
             e,
-            si,
-            ni,
-            Dn, {
+            ao,
+            fo,
+            Xi, {
                 i18n: 1,
                 eta: 0,
                 queue_position: 2,
                 queue_size: 3,
                 status: 4,
                 scroll_to_output: 21,
                 timer: 5,
@@ -3025,115 +3279,115 @@
             },
             null,
             [-1, -1]
         );
     }
 }
 const {
-    SvelteComponent: fi,
-    add_flush_callback: Ot,
-    assign: _i,
-    bind: Rt,
-    binding_callbacks: At,
-    check_outros: ai,
+    SvelteComponent: uo,
+    add_flush_callback: Qt,
+    assign: co,
+    bind: xt,
+    binding_callbacks: $t,
+    check_outros: mo,
     create_component: xe,
     destroy_component: $e,
-    detach: ri,
-    flush: M,
-    get_spread_object: ui,
-    get_spread_update: ci,
-    group_outros: di,
-    init: mi,
-    insert: hi,
+    detach: go,
+    flush: N,
+    get_spread_object: ho,
+    get_spread_update: bo,
+    group_outros: wo,
+    init: vo,
+    insert: po,
     mount_component: et,
-    safe_not_equal: bi,
-    space: gi,
+    safe_not_equal: ko,
+    space: yo,
     transition_in: ye,
-    transition_out: Fe
+    transition_out: He
 } = window.__gradio__svelte__internal;
 
-function Dt(l) {
+function el(l) {
     let e, t;
     const n = [{
             autoscroll: (
                 /*gradio*/
                 l[3].autoscroll
             )
         }, {
             i18n: (
                 /*gradio*/
                 l[3].i18n
             )
         },
         /*loading_status*/
-        l[17]
+        l[18]
     ];
     let i = {};
-    for (let s = 0; s < n.length; s += 1)
-        i = _i(i, n[s]);
-    return e = new oi({
+    for (let o = 0; o < n.length; o += 1)
+        i = co(i, n[o]);
+    return e = new ro({
         props: i
     }), {
         c() {
             xe(e.$$.fragment);
         },
-        m(s, o) {
-            et(e, s, o), t = !0;
+        m(o, s) {
+            et(e, o, s), t = !0;
         },
-        p(s, o) {
-            const r = o & /*gradio, loading_status*/
-                131080 ? ci(n, [
-                    o & /*gradio*/
+        p(o, s) {
+            const f = s[0] & /*gradio, loading_status*/
+                262152 ? bo(n, [
+                    s[0] & /*gradio*/
                     8 && {
                         autoscroll: (
                             /*gradio*/
-                            s[3].autoscroll
+                            o[3].autoscroll
                         )
                     },
-                    o & /*gradio*/
+                    s[0] & /*gradio*/
                     8 && {
                         i18n: (
                             /*gradio*/
-                            s[3].i18n
+                            o[3].i18n
                         )
                     },
-                    o & /*loading_status*/
-                    131072 && ui(
+                    s[0] & /*loading_status*/
+                    262144 && ho(
                         /*loading_status*/
-                        s[17]
+                        o[18]
                     )
                 ]) : {};
-            e.$set(r);
+            e.$set(f);
         },
-        i(s) {
-            t || (ye(e.$$.fragment, s), t = !0);
+        i(o) {
+            t || (ye(e.$$.fragment, o), t = !0);
         },
-        o(s) {
-            Fe(e.$$.fragment, s), t = !1;
+        o(o) {
+            He(e.$$.fragment, o), t = !1;
         },
-        d(s) {
-            $e(e, s);
+        d(o) {
+            $e(e, o);
         }
     };
 }
 
-function wi(l) {
-    let e, t, n, i, s, o = (
+function Co(l) {
+    let e, t, n, i, o, s = (
         /*loading_status*/
-        l[17] && Dt(l)
+        l[18] && el(l)
     );
 
-    function r(_) {
-        l[22](_);
+    function f(r) {
+        l[23](r);
     }
 
-    function a(_) {
-        l[23](_);
+    function a(r) {
+        l[24](r);
     }
-    let f = {
+    let _ = {
         label: (
             /*label*/
             l[4]
         ),
         info: (
             /*info*/
             l[6]
@@ -3158,108 +3412,118 @@
             /*color_map*/
             l[1]
         ),
         show_copy_button: (
             /*show_copy_button*/
             l[16]
         ),
+        show_remove_tags_button: (
+            /*show_remove_tags_button*/
+            l[17]
+        ),
         container: (
             /*container*/
             l[13]
         ),
         disabled: ! /*interactive*/
-            l[18]
+            l[19]
     };
     return (
         /*value*/
-        l[0] !== void 0 && (f.value = /*value*/
+        l[0] !== void 0 && (_.value = /*value*/
             l[0]), /*value_is_output*/
-        l[2] !== void 0 && (f.value_is_output = /*value_is_output*/
-            l[2]), t = new fn({
-            props: f
-        }), At.push(() => Rt(t, "value", r)), At.push(() => Rt(t, "value_is_output", a)), t.$on(
+        l[2] !== void 0 && (_.value_is_output = /*value_is_output*/
+            l[2]), t = new ui({
+            props: _
+        }), $t.push(() => xt(t, "value", f)), $t.push(() => xt(t, "value_is_output", a)), t.$on(
             "change",
             /*change_handler*/
-            l[24]
+            l[25]
         ), t.$on(
             "input",
             /*input_handler*/
-            l[25]
+            l[26]
         ), t.$on(
             "submit",
             /*submit_handler*/
-            l[26]
+            l[27]
         ), t.$on(
             "blur",
             /*blur_handler*/
-            l[27]
+            l[28]
         ), t.$on(
             "select",
             /*select_handler*/
-            l[28]
+            l[29]
         ), t.$on(
             "focus",
             /*focus_handler*/
-            l[29]
+            l[30]
+        ), t.$on(
+            "clear",
+            /*clear_handler*/
+            l[31]
         ), {
             c() {
-                o && o.c(), e = gi(), xe(t.$$.fragment);
+                s && s.c(), e = yo(), xe(t.$$.fragment);
             },
-            m(_, u) {
-                o && o.m(_, u), hi(_, e, u), et(t, _, u), s = !0;
+            m(r, u) {
+                s && s.m(r, u), po(r, e, u), et(t, r, u), o = !0;
             },
-            p(_, u) {
+            p(r, u) {
                 /*loading_status*/
-                _[17] ? o ? (o.p(_, u), u & /*loading_status*/
-                    131072 && ye(o, 1)) : (o = Dt(_), o.c(), ye(o, 1), o.m(e.parentNode, e)) : o && (di(), Fe(o, 1, 1, () => {
-                    o = null;
-                }), ai());
+                r[18] ? s ? (s.p(r, u), u[0] & /*loading_status*/
+                    262144 && ye(s, 1)) : (s = el(r), s.c(), ye(s, 1), s.m(e.parentNode, e)) : s && (wo(), He(s, 1, 1, () => {
+                    s = null;
+                }), mo());
                 const c = {};
-                u & /*label*/
+                u[0] & /*label*/
                     16 && (c.label = /*label*/
-                        _[4]), u & /*info*/
+                        r[4]), u[0] & /*info*/
                     64 && (c.info = /*info*/
-                        _[6]), u & /*show_label*/
+                        r[6]), u[0] & /*show_label*/
                     1024 && (c.show_label = /*show_label*/
-                        _[10]), u & /*show_legend*/
+                        r[10]), u[0] & /*show_legend*/
                     2048 && (c.show_legend = /*show_legend*/
-                        _[11]), u & /*show_legend_label*/
+                        r[11]), u[0] & /*show_legend_label*/
                     4096 && (c.show_legend_label = /*show_legend_label*/
-                        _[12]), u & /*legend_label*/
+                        r[12]), u[0] & /*legend_label*/
                     32 && (c.legend_label = /*legend_label*/
-                        _[5]), u & /*color_map*/
+                        r[5]), u[0] & /*color_map*/
                     2 && (c.color_map = /*color_map*/
-                        _[1]), u & /*show_copy_button*/
+                        r[1]), u[0] & /*show_copy_button*/
                     65536 && (c.show_copy_button = /*show_copy_button*/
-                        _[16]), u & /*container*/
+                        r[16]), u[0] & /*show_remove_tags_button*/
+                    131072 && (c.show_remove_tags_button = /*show_remove_tags_button*/
+                        r[17]), u[0] & /*container*/
                     8192 && (c.container = /*container*/
-                        _[13]), u & /*interactive*/
-                    262144 && (c.disabled = ! /*interactive*/
-                        _[18]), !n && u & /*value*/
+                        r[13]), u[0] & /*interactive*/
+                    524288 && (c.disabled = ! /*interactive*/
+                        r[19]), !n && u[0] & /*value*/
                     1 && (n = !0, c.value = /*value*/
-                        _[0], Ot(() => n = !1)), !i && u & /*value_is_output*/
+                        r[0], Qt(() => n = !1)), !i && u[0] & /*value_is_output*/
                     4 && (i = !0, c.value_is_output = /*value_is_output*/
-                        _[2], Ot(() => i = !1)), t.$set(c);
+                        r[2], Qt(() => i = !1)), t.$set(c);
             },
-            i(_) {
-                s || (ye(o), ye(t.$$.fragment, _), s = !0);
+            i(r) {
+                o || (ye(s), ye(t.$$.fragment, r), o = !0);
             },
-            o(_) {
-                Fe(o), Fe(t.$$.fragment, _), s = !1;
+            o(r) {
+                He(s), He(t.$$.fragment, r), o = !1;
             },
-            d(_) {
-                _ && ri(e), o && o.d(_), $e(t, _);
+            d(r) {
+                r && go(e), s && s.d(r), $e(t, r);
             }
         }
     );
 }
 
-function ki(l) {
+function qo(l) {
     let e, t;
-    return e = new Cn({
+    return e = new Li({
         props: {
             visible: (
                 /*visible*/
                 l[9]
             ),
             elem_id: (
                 /*elem_id*/
@@ -3279,347 +3543,372 @@
             ),
             allow_overflow: !1,
             padding: (
                 /*container*/
                 l[13]
             ),
             $$slots: {
-                default: [wi]
+                default: [Co]
             },
             $$scope: {
                 ctx: l
             }
         }
     }), {
         c() {
             xe(e.$$.fragment);
         },
         m(n, i) {
             et(e, n, i), t = !0;
         },
-        p(n, [i]) {
-            const s = {};
-            i & /*visible*/
-                512 && (s.visible = /*visible*/
-                    n[9]), i & /*elem_id*/
-                128 && (s.elem_id = /*elem_id*/
-                    n[7]), i & /*elem_classes*/
-                256 && (s.elem_classes = /*elem_classes*/
-                    n[8]), i & /*scale*/
-                16384 && (s.scale = /*scale*/
-                    n[14]), i & /*min_width*/
-                32768 && (s.min_width = /*min_width*/
-                    n[15]), i & /*container*/
-                8192 && (s.padding = /*container*/
-                    n[13]), i & /*$$scope, label, info, show_label, show_legend, show_legend_label, legend_label, color_map, show_copy_button, container, interactive, value, value_is_output, gradio, loading_status*/
-                1074216063 && (s.$$scope = {
+        p(n, i) {
+            const o = {};
+            i[0] & /*visible*/
+                512 && (o.visible = /*visible*/
+                    n[9]), i[0] & /*elem_id*/
+                128 && (o.elem_id = /*elem_id*/
+                    n[7]), i[0] & /*elem_classes*/
+                256 && (o.elem_classes = /*elem_classes*/
+                    n[8]), i[0] & /*scale*/
+                16384 && (o.scale = /*scale*/
+                    n[14]), i[0] & /*min_width*/
+                32768 && (o.min_width = /*min_width*/
+                    n[15]), i[0] & /*container*/
+                8192 && (o.padding = /*container*/
+                    n[13]), i[0] & /*label, info, show_label, show_legend, show_legend_label, legend_label, color_map, show_copy_button, show_remove_tags_button, container, interactive, value, value_is_output, gradio, loading_status*/
+                998527 | i[1] & /*$$scope*/
+                2 && (o.$$scope = {
                     dirty: i,
                     ctx: n
-                }), e.$set(s);
+                }), e.$set(o);
         },
         i(n) {
             t || (ye(e.$$.fragment, n), t = !0);
         },
         o(n) {
-            Fe(e.$$.fragment, n), t = !1;
+            He(e.$$.fragment, n), t = !1;
         },
         d(n) {
             $e(e, n);
         }
     };
 }
 
-function vi(l, e, t) {
+function To(l, e, t) {
     let {
         gradio: n
     } = e, {
         label: i = "Highlighted Textbox"
     } = e, {
-        legend_label: s = "Highlights:"
+        legend_label: o = "Highlights:"
     } = e, {
-        info: o = void 0
+        info: s = void 0
     } = e, {
-        elem_id: r = ""
+        elem_id: f = ""
     } = e, {
         elem_classes: a = []
     } = e, {
-        visible: f = !0
+        visible: _ = !0
     } = e, {
-        value: _
+        value: r
     } = e, {
         show_label: u
     } = e, {
         show_legend: c
     } = e, {
         show_legend_label: m
     } = e, {
-        color_map: y = {}
+        color_map: k = {}
+    } = e, {
+        container: L = !0
     } = e, {
-        container: S = !0
+        scale: S = null
     } = e, {
-        scale: T = null
+        min_width: T = void 0
     } = e, {
-        min_width: L = void 0
+        show_copy_button: y = !1
     } = e, {
-        show_copy_button: C = !1
+        show_remove_tags_button: d = !1
     } = e, {
-        loading_status: d = void 0
+        loading_status: C = void 0
     } = e, {
-        value_is_output: p = !1
+        value_is_output: j = !1
     } = e, {
-        combine_adjacent: H = !1
+        combine_adjacent: h = !1
     } = e, {
-        interactive: b = !0
+        interactive: Z = !0
     } = e;
-    const R = !1,
-        K = !0;
+    const J = !1,
+        E = !0;
 
-    function E(g) {
-        _ = g, t(0, _), t(19, H);
+    function O(b) {
+        r = b, t(0, r), t(20, h);
     }
 
-    function A(g) {
-        p = g, t(2, p);
-    }
-    const X = () => n.dispatch("change"),
-        he = () => n.dispatch("input"),
-        D = () => n.dispatch("submit"),
-        Q = () => n.dispatch("blur"),
-        P = (g) => n.dispatch("select", g.detail),
-        be = () => n.dispatch("focus");
-    return l.$$set = (g) => {
-        "gradio" in g && t(3, n = g.gradio), "label" in g && t(4, i = g.label), "legend_label" in g && t(5, s = g.legend_label), "info" in g && t(6, o = g.info), "elem_id" in g && t(7, r = g.elem_id), "elem_classes" in g && t(8, a = g.elem_classes), "visible" in g && t(9, f = g.visible), "value" in g && t(0, _ = g.value), "show_label" in g && t(10, u = g.show_label), "show_legend" in g && t(11, c = g.show_legend), "show_legend_label" in g && t(12, m = g.show_legend_label), "color_map" in g && t(1, y = g.color_map), "container" in g && t(13, S = g.container), "scale" in g && t(14, T = g.scale), "min_width" in g && t(15, L = g.min_width), "show_copy_button" in g && t(16, C = g.show_copy_button), "loading_status" in g && t(17, d = g.loading_status), "value_is_output" in g && t(2, p = g.value_is_output), "combine_adjacent" in g && t(19, H = g.combine_adjacent), "interactive" in g && t(18, b = g.interactive);
+    function R(b) {
+        j = b, t(2, j);
+    }
+    const ae = () => n.dispatch("change"),
+        A = () => n.dispatch("input"),
+        K = () => n.dispatch("submit"),
+        D = () => n.dispatch("blur"),
+        me = (b) => n.dispatch("select", b.detail),
+        Le = () => n.dispatch("focus"),
+        ge = function() {
+            console.log("test"), n.dispatch("clear");
+        };
+    return l.$$set = (b) => {
+        "gradio" in b && t(3, n = b.gradio), "label" in b && t(4, i = b.label), "legend_label" in b && t(5, o = b.legend_label), "info" in b && t(6, s = b.info), "elem_id" in b && t(7, f = b.elem_id), "elem_classes" in b && t(8, a = b.elem_classes), "visible" in b && t(9, _ = b.visible), "value" in b && t(0, r = b.value), "show_label" in b && t(10, u = b.show_label), "show_legend" in b && t(11, c = b.show_legend), "show_legend_label" in b && t(12, m = b.show_legend_label), "color_map" in b && t(1, k = b.color_map), "container" in b && t(13, L = b.container), "scale" in b && t(14, S = b.scale), "min_width" in b && t(15, T = b.min_width), "show_copy_button" in b && t(16, y = b.show_copy_button), "show_remove_tags_button" in b && t(17, d = b.show_remove_tags_button), "loading_status" in b && t(18, C = b.loading_status), "value_is_output" in b && t(2, j = b.value_is_output), "combine_adjacent" in b && t(20, h = b.combine_adjacent), "interactive" in b && t(19, Z = b.interactive);
     }, l.$$.update = () => {
-        l.$$.dirty & /*color_map*/
-            2 && !y && Object.keys(y).length && t(1, y), l.$$.dirty & /*value, combine_adjacent*/
-            524289 && _ && H && t(0, _ = Ol(_, "equal"));
+        l.$$.dirty[0] & /*color_map*/
+            2 && !k && Object.keys(k).length && t(1, k), l.$$.dirty[0] & /*value, combine_adjacent*/
+            1048577 && r && h && t(0, r = Gn(r, "equal"));
     }, [
-        _,
-        y,
-        p,
+        r,
+        k,
+        j,
         n,
         i,
-        s,
         o,
-        r,
-        a,
+        s,
         f,
+        a,
+        _,
         u,
         c,
         m,
+        L,
         S,
         T,
-        L,
-        C,
+        y,
         d,
-        b,
-        H,
-        R,
-        K,
+        C,
+        Z,
+        h,
+        J,
         E,
+        O,
+        R,
+        ae,
         A,
-        X,
-        he,
+        K,
         D,
-        Q,
-        P,
-        be
+        me,
+        Le,
+        ge
     ];
 }
-class pi extends fi {
+class So extends uo {
     constructor(e) {
-        super(), mi(this, e, vi, ki, bi, {
-            gradio: 3,
-            label: 4,
-            legend_label: 5,
-            info: 6,
-            elem_id: 7,
-            elem_classes: 8,
-            visible: 9,
-            value: 0,
-            show_label: 10,
-            show_legend: 11,
-            show_legend_label: 12,
-            color_map: 1,
-            container: 13,
-            scale: 14,
-            min_width: 15,
-            show_copy_button: 16,
-            loading_status: 17,
-            value_is_output: 2,
-            combine_adjacent: 19,
-            interactive: 18,
-            autofocus: 20,
-            autoscroll: 21
-        });
+        super(), vo(
+            this,
+            e,
+            To,
+            qo,
+            ko, {
+                gradio: 3,
+                label: 4,
+                legend_label: 5,
+                info: 6,
+                elem_id: 7,
+                elem_classes: 8,
+                visible: 9,
+                value: 0,
+                show_label: 10,
+                show_legend: 11,
+                show_legend_label: 12,
+                color_map: 1,
+                container: 13,
+                scale: 14,
+                min_width: 15,
+                show_copy_button: 16,
+                show_remove_tags_button: 17,
+                loading_status: 18,
+                value_is_output: 2,
+                combine_adjacent: 20,
+                interactive: 19,
+                autofocus: 21,
+                autoscroll: 22
+            },
+            null,
+            [-1, -1]
+        );
     }
     get gradio() {
         return this.$$.ctx[3];
     }
     set gradio(e) {
         this.$$set({
             gradio: e
-        }), M();
+        }), N();
     }
     get label() {
         return this.$$.ctx[4];
     }
     set label(e) {
         this.$$set({
             label: e
-        }), M();
+        }), N();
     }
     get legend_label() {
         return this.$$.ctx[5];
     }
     set legend_label(e) {
         this.$$set({
             legend_label: e
-        }), M();
+        }), N();
     }
     get info() {
         return this.$$.ctx[6];
     }
     set info(e) {
         this.$$set({
             info: e
-        }), M();
+        }), N();
     }
     get elem_id() {
         return this.$$.ctx[7];
     }
     set elem_id(e) {
         this.$$set({
             elem_id: e
-        }), M();
+        }), N();
     }
     get elem_classes() {
         return this.$$.ctx[8];
     }
     set elem_classes(e) {
         this.$$set({
             elem_classes: e
-        }), M();
+        }), N();
     }
     get visible() {
         return this.$$.ctx[9];
     }
     set visible(e) {
         this.$$set({
             visible: e
-        }), M();
+        }), N();
     }
     get value() {
         return this.$$.ctx[0];
     }
     set value(e) {
         this.$$set({
             value: e
-        }), M();
+        }), N();
     }
     get show_label() {
         return this.$$.ctx[10];
     }
     set show_label(e) {
         this.$$set({
             show_label: e
-        }), M();
+        }), N();
     }
     get show_legend() {
         return this.$$.ctx[11];
     }
     set show_legend(e) {
         this.$$set({
             show_legend: e
-        }), M();
+        }), N();
     }
     get show_legend_label() {
         return this.$$.ctx[12];
     }
     set show_legend_label(e) {
         this.$$set({
             show_legend_label: e
-        }), M();
+        }), N();
     }
     get color_map() {
         return this.$$.ctx[1];
     }
     set color_map(e) {
         this.$$set({
             color_map: e
-        }), M();
+        }), N();
     }
     get container() {
         return this.$$.ctx[13];
     }
     set container(e) {
         this.$$set({
             container: e
-        }), M();
+        }), N();
     }
     get scale() {
         return this.$$.ctx[14];
     }
     set scale(e) {
         this.$$set({
             scale: e
-        }), M();
+        }), N();
     }
     get min_width() {
         return this.$$.ctx[15];
     }
     set min_width(e) {
         this.$$set({
             min_width: e
-        }), M();
+        }), N();
     }
     get show_copy_button() {
         return this.$$.ctx[16];
     }
     set show_copy_button(e) {
         this.$$set({
             show_copy_button: e
-        }), M();
+        }), N();
     }
-    get loading_status() {
+    get show_remove_tags_button() {
         return this.$$.ctx[17];
     }
+    set show_remove_tags_button(e) {
+        this.$$set({
+            show_remove_tags_button: e
+        }), N();
+    }
+    get loading_status() {
+        return this.$$.ctx[18];
+    }
     set loading_status(e) {
         this.$$set({
             loading_status: e
-        }), M();
+        }), N();
     }
     get value_is_output() {
         return this.$$.ctx[2];
     }
     set value_is_output(e) {
         this.$$set({
             value_is_output: e
-        }), M();
+        }), N();
     }
     get combine_adjacent() {
-        return this.$$.ctx[19];
+        return this.$$.ctx[20];
     }
     set combine_adjacent(e) {
         this.$$set({
             combine_adjacent: e
-        }), M();
+        }), N();
     }
     get interactive() {
-        return this.$$.ctx[18];
+        return this.$$.ctx[19];
     }
     set interactive(e) {
         this.$$set({
             interactive: e
-        }), M();
+        }), N();
     }
     get autofocus() {
-        return this.$$.ctx[20];
+        return this.$$.ctx[21];
     }
     get autoscroll() {
-        return this.$$.ctx[21];
+        return this.$$.ctx[22];
     }
 }
 export {
-    pi as
+    So as
     default
 };
```

### Comparing `gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/templates/component/style.css` & `gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/templates/component/style.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-span.has-info.svelte-vm3q5z{margin-bottom:var(--spacing-xs)}span.svelte-vm3q5z:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-vm3q5z{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-vm3q5z{display:none!important}.category-legend.svelte-vm3q5z{display:flex;flex-wrap:wrap;gap:var(--spacing-sm);color:#000}.category-label.svelte-vm3q5z{border-radius:var(--radius-xs);padding-right:var(--size-2);padding-left:var(--size-2);font-weight:var(--weight-semibold)}.category-label.has-info.svelte-vm3q5z{margin-bottom:var(--spacing-xs)}.category-label.svelte-vm3q5z:not(.has-info){margin-bottom:var(--spacing-lg)}.title-container.svelte-vm3q5z{display:flex}.legend-separator.svelte-vm3q5z{margin:0 var(--spacing-md) 0 var(--spacing-md)}.title-with-highlights-info.svelte-vm3q5z{margin-bottom:var(--spacing-xs);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}.dropdown-arrow.svelte-145leq6{fill:currentColor}label.svelte-40uavx{display:block;width:100%}button.svelte-40uavx{display:flex;position:absolute;top:var(--block-label-margin);right:var(--block-label-margin);align-items:center;box-shadow:var(--shadow-drop);border:1px solid var(--color-border-primary);border-top:none;border-right:none;border-radius:var(--block-label-right-radius);background:var(--block-label-background-fill);padding:5px;width:22px;height:22px;overflow:hidden;color:var(--block-label-color);font:var(--font-sans);font-size:var(--button-small-text-size)}.container.svelte-40uavx{display:flex;flex-direction:column;gap:var(--spacing-sm)}.textfield.svelte-40uavx{box-sizing:border-box;outline:none!important;box-shadow:var(--input-shadow);padding:var(--input-padding);border-radius:var(--radius-md);background:var(--input-background-fill);background-color:transparent;font-weight:var(--input-text-weight);font-size:var(--input-text-size);width:100%;line-height:var(--line-sm);word-break:break-word;border:var(--input-border-width) solid var(--input-border-color);cursor:text;white-space:break-spaces}.textfield.svelte-40uavx:focus{box-shadow:var(--input-shadow-focus);border-color:var(--input-border-color-focus)}mark{border-radius:3px}.block.svelte-1t38q2d{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-1t38q2d{border-color:var(--color-accent)}.padded.svelte-1t38q2d{padding:var(--block-padding)}.hidden.svelte-1t38q2d{display:none}.hide-container.svelte-1t38q2d{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-1txqlrd.svelte-1txqlrd{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden;pointer-events:none}.wrap.center.svelte-1txqlrd.svelte-1txqlrd{top:0;right:0;left:0}.wrap.default.svelte-1txqlrd.svelte-1txqlrd{top:0;right:0;bottom:0;left:0}.hide.svelte-1txqlrd.svelte-1txqlrd{opacity:0;pointer-events:none}.generating.svelte-1txqlrd.svelte-1txqlrd{animation:svelte-1txqlrd-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent}.translucent.svelte-1txqlrd.svelte-1txqlrd{background:none}@keyframes svelte-1txqlrd-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-1txqlrd.svelte-1txqlrd{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-1txqlrd.svelte-1txqlrd{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-1txqlrd.svelte-1txqlrd{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-1txqlrd.svelte-1txqlrd{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-1txqlrd.svelte-1txqlrd{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-1txqlrd.svelte-1txqlrd{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-1txqlrd.svelte-1txqlrd{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-1txqlrd.svelte-1txqlrd{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-1txqlrd.svelte-1txqlrd{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-1txqlrd .progress-text.svelte-1txqlrd{background:var(--block-background-fill)}.border.svelte-1txqlrd.svelte-1txqlrd{border:1px solid var(--border-color-primary)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}
+span.has-info.svelte-vm3q5z{margin-bottom:var(--spacing-xs)}span.svelte-vm3q5z:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-vm3q5z{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-vm3q5z{display:none!important}.category-legend.svelte-vm3q5z{display:flex;flex-wrap:wrap;gap:var(--spacing-sm);color:#000}.category-label.svelte-vm3q5z{border-radius:var(--radius-xs);padding-right:var(--size-2);padding-left:var(--size-2);font-weight:var(--weight-semibold)}.category-label.has-info.svelte-vm3q5z{margin-bottom:var(--spacing-xs)}.category-label.svelte-vm3q5z:not(.has-info){margin-bottom:var(--spacing-lg)}.title-container.svelte-vm3q5z{display:flex}.legend-separator.svelte-vm3q5z{margin:0 var(--spacing-md) 0 var(--spacing-md)}.title-with-highlights-info.svelte-vm3q5z{margin-bottom:var(--spacing-xs);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}.dropdown-arrow.svelte-145leq6{fill:currentColor}button.svelte-qjb524{position:relative;cursor:pointer;padding:5px;width:22px;height:22px}.check.svelte-qjb524{position:absolute;top:0;right:0;z-index:var(--layer-top);background:var(--background-fill-primary);padding:var(--size-1);width:100%;height:100%;color:var(--body-text-color)}button.svelte-1ga0gmr{position:relative;cursor:pointer;padding:5px;width:22px;height:22px;background-color:green}div.svelte-1bqqv16{display:flex;position:absolute;top:var(--block-label-margin);right:var(--block-label-margin);align-items:center;z-index:var(--layer-2);transition:.15s;box-shadow:var(--shadow-drop);border:1px solid var(--border-color-primary);border-top:none;border-right:none;border-radius:var(--block-label-right-radius);background:var(--block-label-background-fill);overflow:hidden;color:var(--block-label-text-color);font:var(--font);font-size:var(--button-small-text-size)}label.svelte-1atky07{display:block;width:100%}.container.svelte-1atky07{display:flex;flex-direction:column;gap:var(--spacing-sm)}.textfield.svelte-1atky07{box-sizing:border-box;outline:none!important;box-shadow:var(--input-shadow);padding:var(--input-padding);border-radius:var(--radius-md);background:var(--input-background-fill);background-color:transparent;font-weight:var(--input-text-weight);font-size:var(--input-text-size);width:100%;line-height:var(--line-sm);word-break:break-word;border:var(--input-border-width) solid var(--input-border-color);cursor:text;white-space:break-spaces}.textfield.svelte-1atky07:focus{box-shadow:var(--input-shadow-focus);border-color:var(--input-border-color-focus)}mark{border-radius:3px}.block.svelte-1t38q2d{position:relative;margin:0;box-shadow:var(--block-shadow);border-width:var(--block-border-width);border-color:var(--block-border-color);border-radius:var(--block-radius);background:var(--block-background-fill);width:100%;line-height:var(--line-sm)}.block.border_focus.svelte-1t38q2d{border-color:var(--color-accent)}.padded.svelte-1t38q2d{padding:var(--block-padding)}.hidden.svelte-1t38q2d{display:none}.hide-container.svelte-1t38q2d{margin:0;box-shadow:none;--block-border-width:0;background:transparent;padding:0;overflow:visible}div.svelte-1hnfib2{margin-bottom:var(--spacing-lg);color:var(--block-info-text-color);font-weight:var(--block-info-text-weight);font-size:var(--block-info-text-size);line-height:var(--line-sm)}span.has-info.svelte-22c38v{margin-bottom:var(--spacing-xs)}span.svelte-22c38v:not(.has-info){margin-bottom:var(--spacing-lg)}span.svelte-22c38v{display:inline-block;position:relative;z-index:var(--layer-4);border:solid var(--block-title-border-width) var(--block-title-border-color);border-radius:var(--block-title-radius);background:var(--block-title-background-fill);padding:var(--block-title-padding);color:var(--block-title-text-color);font-weight:var(--block-title-text-weight);font-size:var(--block-title-text-size);line-height:var(--line-sm)}.hide.svelte-22c38v{margin:0;height:0}label.svelte-9gxdi0{display:inline-flex;align-items:center;z-index:var(--layer-2);box-shadow:var(--block-label-shadow);border:var(--block-label-border-width) solid var(--border-color-primary);border-top:none;border-left:none;border-radius:var(--block-label-radius);background:var(--block-label-background-fill);padding:var(--block-label-padding);pointer-events:none;color:var(--block-label-text-color);font-weight:var(--block-label-text-weight);font-size:var(--block-label-text-size);line-height:var(--line-sm)}.gr-group label.svelte-9gxdi0{border-top-left-radius:0}label.float.svelte-9gxdi0{position:absolute;top:var(--block-label-margin);left:var(--block-label-margin)}label.svelte-9gxdi0:not(.float){position:static;margin-top:var(--block-label-margin);margin-left:var(--block-label-margin)}.hide.svelte-9gxdi0{height:0}span.svelte-9gxdi0{opacity:.8;margin-right:var(--size-2);width:calc(var(--block-label-text-size) - 1px);height:calc(var(--block-label-text-size) - 1px)}.hide-label.svelte-9gxdi0{box-shadow:none;border-width:0;background:transparent;overflow:visible}button.svelte-lpi64a{display:flex;justify-content:center;align-items:center;gap:1px;z-index:var(--layer-2);border-radius:var(--radius-sm);color:var(--block-label-text-color);border:1px solid transparent}button[disabled].svelte-lpi64a{opacity:.5;box-shadow:none}button[disabled].svelte-lpi64a:hover{cursor:not-allowed}.padded.svelte-lpi64a{padding:2px;background:var(--bg-color);box-shadow:var(--shadow-drop);border:1px solid var(--button-secondary-border-color)}button.svelte-lpi64a:hover,button.highlight.svelte-lpi64a{cursor:pointer;color:var(--color-accent)}.padded.svelte-lpi64a:hover{border:2px solid var(--button-secondary-border-color-hover);padding:1px;color:var(--block-label-text-color)}span.svelte-lpi64a{padding:0 1px;font-size:10px}div.svelte-lpi64a{padding:2px;display:flex;align-items:flex-end}.small.svelte-lpi64a{width:14px;height:14px}.large.svelte-lpi64a{width:22px;height:22px}.pending.svelte-lpi64a{animation:svelte-lpi64a-flash .5s infinite}@keyframes svelte-lpi64a-flash{0%{opacity:.5}50%{opacity:1}to{opacity:.5}}.transparent.svelte-lpi64a{background:transparent;border:none;box-shadow:none}.empty.svelte-3w3rth{display:flex;justify-content:center;align-items:center;margin-top:calc(0px - var(--size-6));height:var(--size-full)}.icon.svelte-3w3rth{opacity:.5;height:var(--size-5);color:var(--body-text-color)}.small.svelte-3w3rth{min-height:calc(var(--size-32) - 20px)}.large.svelte-3w3rth{min-height:calc(var(--size-64) - 20px)}.unpadded_box.svelte-3w3rth{margin-top:0}.small_parent.svelte-3w3rth{min-height:100%!important}.wrap.svelte-kzcjhc{display:flex;flex-direction:column;justify-content:center;align-items:center;min-height:var(--size-60);color:var(--block-label-text-color);line-height:var(--line-md);height:100%;padding-top:var(--size-3)}.or.svelte-kzcjhc{color:var(--body-text-color-subdued);display:flex}.icon-wrap.svelte-kzcjhc{width:30px;margin-bottom:var(--spacing-lg)}@media (--screen-md){.wrap.svelte-kzcjhc{font-size:var(--text-lg)}}.hovered.svelte-kzcjhc{color:var(--color-accent)}div.svelte-ipfyu7{border-top:1px solid transparent;display:flex;max-height:100%;justify-content:center;gap:var(--spacing-sm);height:auto;align-items:flex-end;padding-bottom:var(--spacing-xl);color:var(--block-label-text-color);flex-shrink:0;width:95%}.show_border.svelte-ipfyu7{border-top:1px solid var(--block-border-color);margin-top:var(--spacing-xxl);box-shadow:var(--shadow-drop)}.source-selection.svelte-1jp3vgd{display:flex;align-items:center;justify-content:center;border-top:1px solid var(--border-color-primary);width:95%;bottom:0;left:0;right:0;margin-left:auto;margin-right:auto}.icon.svelte-1jp3vgd{width:22px;height:22px;margin:var(--spacing-lg) var(--spacing-xs);padding:var(--spacing-xs);color:var(--neutral-400);border-radius:var(--radius-md)}.selected.svelte-1jp3vgd{color:var(--color-accent)}.icon.svelte-1jp3vgd:hover,.icon.svelte-1jp3vgd:focus{color:var(--color-accent)}svg.svelte-43sxxs.svelte-43sxxs{width:var(--size-20);height:var(--size-20)}svg.svelte-43sxxs path.svelte-43sxxs{fill:var(--loader-color)}div.svelte-43sxxs.svelte-43sxxs{z-index:var(--layer-2)}.margin.svelte-43sxxs.svelte-43sxxs{margin:var(--size-4)}.wrap.svelte-1txqlrd.svelte-1txqlrd{display:flex;flex-direction:column;justify-content:center;align-items:center;z-index:var(--layer-top);transition:opacity .1s ease-in-out;border-radius:var(--block-radius);background:var(--block-background-fill);padding:0 var(--size-6);max-height:var(--size-screen-h);overflow:hidden;pointer-events:none}.wrap.center.svelte-1txqlrd.svelte-1txqlrd{top:0;right:0;left:0}.wrap.default.svelte-1txqlrd.svelte-1txqlrd{top:0;right:0;bottom:0;left:0}.hide.svelte-1txqlrd.svelte-1txqlrd{opacity:0;pointer-events:none}.generating.svelte-1txqlrd.svelte-1txqlrd{animation:svelte-1txqlrd-pulse 2s cubic-bezier(.4,0,.6,1) infinite;border:2px solid var(--color-accent);background:transparent}.translucent.svelte-1txqlrd.svelte-1txqlrd{background:none}@keyframes svelte-1txqlrd-pulse{0%,to{opacity:1}50%{opacity:.5}}.loading.svelte-1txqlrd.svelte-1txqlrd{z-index:var(--layer-2);color:var(--body-text-color)}.eta-bar.svelte-1txqlrd.svelte-1txqlrd{position:absolute;top:0;right:0;bottom:0;left:0;transform-origin:left;opacity:.8;z-index:var(--layer-1);transition:10ms;background:var(--background-fill-secondary)}.progress-bar-wrap.svelte-1txqlrd.svelte-1txqlrd{border:1px solid var(--border-color-primary);background:var(--background-fill-primary);width:55.5%;height:var(--size-4)}.progress-bar.svelte-1txqlrd.svelte-1txqlrd{transform-origin:left;background-color:var(--loader-color);width:var(--size-full);height:var(--size-full)}.progress-level.svelte-1txqlrd.svelte-1txqlrd{display:flex;flex-direction:column;align-items:center;gap:1;z-index:var(--layer-2);width:var(--size-full)}.progress-level-inner.svelte-1txqlrd.svelte-1txqlrd{margin:var(--size-2) auto;color:var(--body-text-color);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text.svelte-1txqlrd.svelte-1txqlrd{position:absolute;top:0;right:0;z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono)}.meta-text-center.svelte-1txqlrd.svelte-1txqlrd{display:flex;position:absolute;top:0;right:0;justify-content:center;align-items:center;transform:translateY(var(--size-6));z-index:var(--layer-2);padding:var(--size-1) var(--size-2);font-size:var(--text-sm);font-family:var(--font-mono);text-align:center}.error.svelte-1txqlrd.svelte-1txqlrd{box-shadow:var(--shadow-drop);border:solid 1px var(--error-border-color);border-radius:var(--radius-full);background:var(--error-background-fill);padding-right:var(--size-4);padding-left:var(--size-4);color:var(--error-text-color);font-weight:var(--weight-semibold);font-size:var(--text-lg);line-height:var(--line-lg);font-family:var(--font)}.minimal.svelte-1txqlrd .progress-text.svelte-1txqlrd{background:var(--block-background-fill)}.border.svelte-1txqlrd.svelte-1txqlrd{border:1px solid var(--border-color-primary)}.toast-body.svelte-solcu7{display:flex;position:relative;right:0;left:0;align-items:center;margin:var(--size-6) var(--size-4);margin:auto;border-radius:var(--container-radius);overflow:hidden;pointer-events:auto}.toast-body.error.svelte-solcu7{border:1px solid var(--color-red-700);background:var(--color-red-50)}.dark .toast-body.error.svelte-solcu7{border:1px solid var(--color-red-500);background-color:var(--color-grey-950)}.toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-700);background:var(--color-yellow-50)}.dark .toast-body.warning.svelte-solcu7{border:1px solid var(--color-yellow-500);background-color:var(--color-grey-950)}.toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-700);background:var(--color-grey-50)}.dark .toast-body.info.svelte-solcu7{border:1px solid var(--color-grey-500);background-color:var(--color-grey-950)}.toast-title.svelte-solcu7{display:flex;align-items:center;font-weight:var(--weight-bold);font-size:var(--text-lg);line-height:var(--line-sm);text-transform:capitalize}.toast-title.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-title.error.svelte-solcu7{color:var(--color-red-50)}.toast-title.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-title.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-title.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-title.info.svelte-solcu7{color:var(--color-grey-50)}.toast-close.svelte-solcu7{margin:0 var(--size-3);border-radius:var(--size-3);padding:0px var(--size-1-5);font-size:var(--size-5);line-height:var(--size-5)}.toast-close.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-close.error.svelte-solcu7{color:var(--color-red-500)}.toast-close.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-close.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-close.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-close.info.svelte-solcu7{color:var(--color-grey-500)}.toast-text.svelte-solcu7{font-size:var(--text-lg)}.toast-text.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-text.error.svelte-solcu7{color:var(--color-red-50)}.toast-text.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-text.warning.svelte-solcu7{color:var(--color-yellow-50)}.toast-text.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-text.info.svelte-solcu7{color:var(--color-grey-50)}.toast-details.svelte-solcu7{margin:var(--size-3) var(--size-3) var(--size-3) 0;width:100%}.toast-icon.svelte-solcu7{display:flex;position:absolute;position:relative;flex-shrink:0;justify-content:center;align-items:center;margin:var(--size-2);border-radius:var(--radius-full);padding:var(--size-1);padding-left:calc(var(--size-1) - 1px);width:35px;height:35px}.toast-icon.error.svelte-solcu7{color:var(--color-red-700)}.dark .toast-icon.error.svelte-solcu7{color:var(--color-red-500)}.toast-icon.warning.svelte-solcu7{color:var(--color-yellow-700)}.dark .toast-icon.warning.svelte-solcu7{color:var(--color-yellow-500)}.toast-icon.info.svelte-solcu7{color:var(--color-grey-700)}.dark .toast-icon.info.svelte-solcu7{color:var(--color-grey-500)}@keyframes svelte-solcu7-countdown{0%{transform:scaleX(1)}to{transform:scaleX(0)}}.timer.svelte-solcu7{position:absolute;bottom:0;left:0;transform-origin:0 0;animation:svelte-solcu7-countdown 10s linear forwards;width:100%;height:var(--size-1)}.timer.error.svelte-solcu7{background:var(--color-red-700)}.dark .timer.error.svelte-solcu7{background:var(--color-red-500)}.timer.warning.svelte-solcu7{background:var(--color-yellow-700)}.dark .timer.warning.svelte-solcu7{background:var(--color-yellow-500)}.timer.info.svelte-solcu7{background:var(--color-grey-700)}.dark .timer.info.svelte-solcu7{background:var(--color-grey-500)}.toast-wrap.svelte-gatr8h{display:flex;position:fixed;top:var(--size-4);right:var(--size-4);flex-direction:column;align-items:end;gap:var(--size-2);z-index:var(--layer-top);width:calc(100% - var(--size-8))}@media (--screen-sm){.toast-wrap.svelte-gatr8h{width:calc(var(--size-96) + var(--size-10))}}
```

### Comparing `gradio_highlightedtextbox-0.0.8/backend/gradio_highlightedtextbox/templates/example/index.js` & `gradio_highlightedtextbox-0.0.9/backend/gradio_highlightedtextbox/templates/example/index.js`

 * *Files identical despite different names*

### Comparing `gradio_highlightedtextbox-0.0.8/demo/app.py` & `gradio_highlightedtextbox-0.0.9/demo/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,40 +32,40 @@
     msg: str,
 ) -> None:
     gr.Info(
         f"{msg}: {HighlightedTextbox.tuples_to_tagged_text(highlighted_text['data'], tag_id, tag_open, tag_close)}"
     )
 
 
-initial_text = "It is not something to be ashamed of: it is no different from the <d>personal fears</d> and <tm>dislikes</tm> of other things that <t>manny peopl</t> have."
+initial_text = "It is not something to be ashamed of: it is no different from the <a>personal fears</a> and <b>dislikes</b> of other things that <c>manny peopl</c> have."
 
 with gr.Blocks() as demo:
     gr.Markdown("### Parameters to control the highlighted textbox:")
     with gr.Row():
         tag_id = gr.Dropdown(
-            choices=["Typo", "Terminology", "Disfluency"],
-            value=["Typo", "Terminology", "Disfluency"],
+            choices=["Error A", "Error B", "Error C"],
+            value=["Error A", "Error B", "Error C"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag ID",
             show_label=True,
             info="Insert one or more tag IDs to use in the highlighted textbox.",
         )
         tag_open = gr.Dropdown(
-            choices=["<t>", "<tm>", "<d>"],
-            value=["<t>", "<tm>", "<d>"],
+            choices=["<a>", "<b>", "<c>"],
+            value=["<a>", "<b>", "<c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag open",
             show_label=True,
             info="Insert one or more tags to mark the beginning of a highlighted section.",
         )
         tag_close = gr.Dropdown(
-            choices=["</t>", "</tm>", "</d>"],
-            value=["</t>", "</tm>", "</d>"],
+            choices=["</a>", "</b>", "</c>"],
+            value=["</a>", "</b>", "</c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag close",
             show_label=True,
             info="Insert one or more tags to mark the end of a highlighted section.",
         )
     gr.Markdown(
@@ -94,14 +94,16 @@
             interactive=True,
             label="Highlighted text",
             info="Textbox containing editable text with custom highlights.",
             show_legend=True,
             show_label=True,
             legend_label="Legend:",
             show_legend_label=True,
+            show_remove_tags_button=True,
+            show_copy_button=False,
         )
 
     # Functions
 
     tagged.input(
         fn=convert_tagged_text_to_highlighted_text,
         inputs=[tagged, tag_id, tag_open, tag_close],
@@ -113,20 +115,20 @@
         outputs=tagged,
     )
     high.focus(
         fn=show_info,
         inputs=[high, tag_id, tag_open, tag_close, gr.State("Focus")],
         outputs=None,
     )
-    high.change(
+    high.blur(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Change")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
         outputs=None,
     )
-    high.blur(
+    high.clear(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Remove tags")],
         outputs=None,
     )
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_highlightedtextbox-0.0.8/demo/css.css` & `gradio_highlightedtextbox-0.0.9/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_highlightedtextbox-0.0.8/demo/space.py` & `gradio_highlightedtextbox-0.0.9/demo/space.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import gradio as gr
 from app import demo as app
 import os
 
-_docs = {'HighlightedTextbox': {'description': 'Creates a textarea for user to enter string input or display string output where some\nelements are highlighted.\n    (1) "text" whose value is the complete text, and\n    (2) "highlights", which is a list of dictionaries, each of which have the keys:\n        "highlight_type" (consisting of the highlight label),\n        "start" (the character index where the label starts), and\n        "end" (the character index where the label ends).\n    Highlights should not overlap.', 'members': {'__init__': {'value': {'type': 'list[tuple[str, str | None]] | Callable | None', 'default': '""', 'description': 'default text to provide in textbox. If callable, the function will be called whenever the app loads to set the initial value of the component.'}, 'color_map': {'type': 'dict[str, str] | None', 'default': 'None', 'description': 'dictionary mapping labels to colors.'}, 'show_legend': {'type': 'bool', 'default': 'False', 'description': 'if True, will display legend.'}, 'show_legend_label': {'type': 'bool', 'default': 'False', 'description': 'if True, will display legend label.'}, 'legend_label': {'type': 'str', 'default': '""', 'description': 'label to display above legend.'}, 'combine_adjacent': {'type': 'bool', 'default': 'False', 'description': 'if True, will combine adjacent spans with the same label.'}, 'adjacent_separator': {'type': 'str', 'default': '""', 'description': 'separator to use when combining adjacent spans.'}, 'label': {'type': 'str | None', 'default': 'None', 'description': 'component name in interface.'}, 'info': {'type': 'str | None', 'default': 'None', 'description': None}, 'every': {'type': 'float | None', 'default': 'None', 'description': "If `value` is a callable, run the function 'every' number of seconds while the client connection is open. Has no effect otherwise. Queue must be enabled. The event can be accessed (e.g. to cancel it) via this component's .load_event attribute."}, 'show_label': {'type': 'bool | None', 'default': 'None', 'description': 'if True, will display label.'}, 'container': {'type': 'bool', 'default': 'True', 'description': 'If True, will place the component in a container - providing some extra padding around the border.'}, 'scale': {'type': 'int | None', 'default': 'None', 'description': 'relative width compared to adjacent Components in a Row. For example, if Component A has scale=2, and Component B has scale=1, A will be twice as wide as B. Should be an integer.'}, 'min_width': {'type': 'int', 'default': '160', 'description': 'minimum pixel width, will wrap if not sufficient screen space to satisfy this value. If a certain scale value results in this Component being narrower than min_width, the min_width parameter will be respected first.'}, 'visible': {'type': 'bool', 'default': 'True', 'description': 'If False, component will be hidden.'}, 'elem_id': {'type': 'str | None', 'default': 'None', 'description': 'An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'autofocus': {'type': 'bool', 'default': 'False', 'description': None}, 'autoscroll': {'type': 'bool', 'default': 'True', 'description': 'If True, will automatically scroll to the bottom of the textbox when the value changes, unless the user scrolls up. If False, will not scroll to the bottom of the textbox when the value changes.'}, 'interactive': {'type': 'bool', 'default': 'True', 'description': 'if True, will be rendered as an editable textbox; if False, editing will be disabled. If not provided, this is inferred based on whether the component is used as an input or output.'}, 'elem_classes': {'type': 'list[str] | str | None', 'default': 'None', 'description': 'An optional list of strings that are assigned as the classes of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'render': {'type': 'bool', 'default': 'True', 'description': 'If False, component will not render be rendered in the Blocks context. Should be used if the intention is to assign event listeners now but render the component later.'}, 'show_copy_button': {'type': 'bool', 'default': 'False', 'description': 'If True, includes a copy button to copy the text in the textbox. Only applies if show_label is True.'}}, 'postprocess': {'y': {'type': 'list[tuple[str, str | None]] | dict | None', 'description': 'List of (word, category) tuples, or a dictionary of two keys: "id", and "data", which is a list of (word, category) tuples.'}, 'value': {'type': 'list[tuple[str, str | None]] | dict | None', 'description': 'List of (word, category) tuples, or a dictionary of two keys: "id", and "data", which is a list of (word, category) tuples.'}}, 'preprocess': {'return': {'type': 'dict', 'description': None}, 'value': None}}, 'events': {'change': {'type': None, 'default': None, 'description': 'Triggered when the value of the HighlightedTextbox changes either because of user input (e.g. a user types in a textbox) OR because of a function update (e.g. an image receives a value from the output of an event trigger). See `.input()` for a listener that is only triggered by user input.'}, 'input': {'type': None, 'default': None, 'description': 'This listener is triggered when the user changes the value of the HighlightedTextbox.'}, 'select': {'type': None, 'default': None, 'description': 'Event listener for when the user selects or deselects the HighlightedTextbox. Uses event data gradio.SelectData to carry `value` referring to the label of the HighlightedTextbox, and `selected` to refer to state of the HighlightedTextbox. See EventData documentation on how to use this event data'}, 'submit': {'type': None, 'default': None, 'description': 'This listener is triggered when the user presses the Enter key while the HighlightedTextbox is focused.'}, 'focus': {'type': None, 'default': None, 'description': 'This listener is triggered when the HighlightedTextbox is focused.'}, 'blur': {'type': None, 'default': None, 'description': 'This listener is triggered when the HighlightedTextbox is unfocused/blurred.'}}}, '__meta__': {'additional_interfaces': {}, 'user_fn_refs': {'HighlightedTextbox': []}}}
+_docs = {'HighlightedTextbox': {'description': 'Creates a textarea for user to enter string input or display string output where some\nelements are highlighted.\n    (1) "text" whose value is the complete text, and\n    (2) "highlights", which is a list of dictionaries, each of which have the keys:\n        "highlight_type" (consisting of the highlight label),\n        "start" (the character index where the label starts), and\n        "end" (the character index where the label ends).\n    Highlights should not overlap.', 'members': {'__init__': {'value': {'type': 'list[tuple[str, str | None]] | Callable | None', 'default': '""', 'description': 'default text to provide in textbox. If callable, the function will be called whenever the app loads to set the initial value of the component.'}, 'color_map': {'type': 'dict[str, str] | None', 'default': 'None', 'description': 'dictionary mapping labels to colors.'}, 'show_legend': {'type': 'bool', 'default': 'False', 'description': 'if True, will display legend.'}, 'show_legend_label': {'type': 'bool', 'default': 'False', 'description': 'if True, will display legend label.'}, 'legend_label': {'type': 'str', 'default': '""', 'description': 'label to display above legend.'}, 'combine_adjacent': {'type': 'bool', 'default': 'False', 'description': 'if True, will combine adjacent spans with the same label.'}, 'adjacent_separator': {'type': 'str', 'default': '""', 'description': 'separator to use when combining adjacent spans.'}, 'label': {'type': 'str | None', 'default': 'None', 'description': 'component name in interface.'}, 'info': {'type': 'str | None', 'default': 'None', 'description': None}, 'every': {'type': 'float | None', 'default': 'None', 'description': "If `value` is a callable, run the function 'every' number of seconds while the client connection is open. Has no effect otherwise. Queue must be enabled. The event can be accessed (e.g. to cancel it) via this component's .load_event attribute."}, 'show_label': {'type': 'bool | None', 'default': 'None', 'description': 'if True, will display label.'}, 'container': {'type': 'bool', 'default': 'True', 'description': 'If True, will place the component in a container - providing some extra padding around the border.'}, 'scale': {'type': 'int | None', 'default': 'None', 'description': 'relative width compared to adjacent Components in a Row. For example, if Component A has scale=2, and Component B has scale=1, A will be twice as wide as B. Should be an integer.'}, 'min_width': {'type': 'int', 'default': '160', 'description': 'minimum pixel width, will wrap if not sufficient screen space to satisfy this value. If a certain scale value results in this Component being narrower than min_width, the min_width parameter will be respected first.'}, 'visible': {'type': 'bool', 'default': 'True', 'description': 'If False, component will be hidden.'}, 'elem_id': {'type': 'str | None', 'default': 'None', 'description': 'An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'autofocus': {'type': 'bool', 'default': 'False', 'description': None}, 'autoscroll': {'type': 'bool', 'default': 'True', 'description': 'If True, will automatically scroll to the bottom of the textbox when the value changes, unless the user scrolls up. If False, will not scroll to the bottom of the textbox when the value changes.'}, 'interactive': {'type': 'bool', 'default': 'True', 'description': 'if True, will be rendered as an editable textbox; if False, editing will be disabled. If not provided, this is inferred based on whether the component is used as an input or output.'}, 'elem_classes': {'type': 'list[str] | str | None', 'default': 'None', 'description': 'An optional list of strings that are assigned as the classes of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'render': {'type': 'bool', 'default': 'True', 'description': 'If False, component will not render be rendered in the Blocks context. Should be used if the intention is to assign event listeners now but render the component later.'}, 'show_copy_button': {'type': 'bool', 'default': 'False', 'description': 'If True, includes a copy button to copy the text in the textbox. Only applies if show_label is True.'}, 'show_remove_tags_button': {'type': 'bool', 'default': 'False', 'description': 'If True, includes a button to remove all tags from the text.'}}, 'postprocess': {'y': {'type': 'list[tuple[str, str | None]] | dict | None', 'description': 'List of (word, category) tuples, or a dictionary of two keys: "id", and "data", which is a list of (word, category) tuples.'}, 'value': {'type': 'list[tuple[str, str | None]] | dict | None', 'description': 'List of (word, category) tuples, or a dictionary of two keys: "id", and "data", which is a list of (word, category) tuples.'}}, 'preprocess': {'return': {'type': 'dict', 'description': None}, 'value': None}}, 'events': {'change': {'type': None, 'default': None, 'description': 'Triggered when the value of the HighlightedTextbox changes either because of user input (e.g. a user types in a textbox) OR because of a function update (e.g. an image receives a value from the output of an event trigger). See `.input()` for a listener that is only triggered by user input.'}, 'input': {'type': None, 'default': None, 'description': 'This listener is triggered when the user changes the value of the HighlightedTextbox.'}, 'select': {'type': None, 'default': None, 'description': 'Event listener for when the user selects or deselects the HighlightedTextbox. Uses event data gradio.SelectData to carry `value` referring to the label of the HighlightedTextbox, and `selected` to refer to state of the HighlightedTextbox. See EventData documentation on how to use this event data'}, 'submit': {'type': None, 'default': None, 'description': 'This listener is triggered when the user presses the Enter key while the HighlightedTextbox is focused.'}, 'focus': {'type': None, 'default': None, 'description': 'This listener is triggered when the HighlightedTextbox is focused.'}, 'blur': {'type': None, 'default': None, 'description': 'This listener is triggered when the HighlightedTextbox is unfocused/blurred.'}, 'clear': {'type': None, 'default': None, 'description': 'This listener is triggered when the user clears the HighlightedTextbox using the X button for the component.'}}}, '__meta__': {'additional_interfaces': {}, 'user_fn_refs': {'HighlightedTextbox': []}}}
     
 abs_path = os.path.join(os.path.dirname(__file__), "css.css")
 
 with gr.Blocks(
     css=abs_path,
     theme=gr.themes.Default(
         font_mono=[
@@ -72,40 +72,40 @@
     msg: str,
 ) -> None:
     gr.Info(
         f"{msg}: {HighlightedTextbox.tuples_to_tagged_text(highlighted_text['data'], tag_id, tag_open, tag_close)}"
     )
 
 
-initial_text = "It is not something to be ashamed of: it is no different from the <d>personal fears</d> and <tm>dislikes</tm> of other things that <t>manny peopl</t> have."
+initial_text = "It is not something to be ashamed of: it is no different from the <a>personal fears</a> and <b>dislikes</b> of other things that <c>manny peopl</c> have."
 
 with gr.Blocks() as demo:
     gr.Markdown("### Parameters to control the highlighted textbox:")
     with gr.Row():
         tag_id = gr.Dropdown(
-            choices=["Typo", "Terminology", "Disfluency"],
-            value=["Typo", "Terminology", "Disfluency"],
+            choices=["Error A", "Error B", "Error C"],
+            value=["Error A", "Error B", "Error C"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag ID",
             show_label=True,
             info="Insert one or more tag IDs to use in the highlighted textbox.",
         )
         tag_open = gr.Dropdown(
-            choices=["<t>", "<tm>", "<d>"],
-            value=["<t>", "<tm>", "<d>"],
+            choices=["<a>", "<b>", "<c>"],
+            value=["<a>", "<b>", "<c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag open",
             show_label=True,
             info="Insert one or more tags to mark the beginning of a highlighted section.",
         )
         tag_close = gr.Dropdown(
-            choices=["</t>", "</tm>", "</d>"],
-            value=["</t>", "</tm>", "</d>"],
+            choices=["</a>", "</b>", "</c>"],
+            value=["</a>", "</b>", "</c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag close",
             show_label=True,
             info="Insert one or more tags to mark the end of a highlighted section.",
         )
     gr.Markdown(
@@ -134,14 +134,16 @@
             interactive=True,
             label="Highlighted text",
             info="Textbox containing editable text with custom highlights.",
             show_legend=True,
             show_label=True,
             legend_label="Legend:",
             show_legend_label=True,
+            show_remove_tags_button=True,
+            show_copy_button=False,
         )
 
     # Functions
 
     tagged.input(
         fn=convert_tagged_text_to_highlighted_text,
         inputs=[tagged, tag_id, tag_open, tag_close],
@@ -153,22 +155,22 @@
         outputs=tagged,
     )
     high.focus(
         fn=show_info,
         inputs=[high, tag_id, tag_open, tag_close, gr.State("Focus")],
         outputs=None,
     )
-    high.change(
+    high.blur(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Change")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
         outputs=None,
     )
-    high.blur(
+    high.clear(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Remove tags")],
         outputs=None,
     )
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
```

### Comparing `gradio_highlightedtextbox-0.0.8/frontend/BlockTitleWithHighlights.svelte` & `gradio_highlightedtextbox-0.0.9/frontend/BlockTitleWithHighlights.svelte`

 * *Files identical despite different names*

### Comparing `gradio_highlightedtextbox-0.0.8/frontend/Example.svelte` & `gradio_highlightedtextbox-0.0.9/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_highlightedtextbox-0.0.8/frontend/HighlightedTextbox.svelte` & `gradio_highlightedtextbox-0.0.9/frontend/HighlightedTextbox.svelte`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 <script lang="ts">
 	import {
 		beforeUpdate,
 		afterUpdate,
 		createEventDispatcher,
 	} from "svelte";
 	import BlockTitleWithHighlights from "./BlockTitleWithHighlights.svelte";
-	import { Copy, Check } from "@gradio/icons";
-	import { fade } from "svelte/transition";
+	import Widgets from "./Widgets.svelte";
 	import type { SelectData } from "@gradio/utils";
 	import { get_next_color } from "@gradio/utils";
 	import { correct_color_map, getParentCursorPosition, getNodeAndOffset } from "./utils";
 
 	const browser = typeof document !== "undefined";
 	export let value: [string, string | null][] = [];
     export let value_is_output: boolean = false;
@@ -19,25 +18,28 @@
 	export let info: string | undefined = undefined;
 	export let show_label = true;
 	export let show_legend = false;
 	export let show_legend_label = false;
 	export let container = true;
 	export let color_map: Record<string, string> = {};
 	export let show_copy_button = false;
+	export let show_remove_tags_button = false;
     export let disabled: boolean;
 	
 	let el: HTMLDivElement;
 	let el_text: string = "";
 	let marked_el_text: string = "";
 	let ctx: CanvasRenderingContext2D;
 	let current_color_map: Record<string, string> = !color_map || Object.keys(color_map).length === 0 ? {} : color_map;
 	let _color_map: Record<string, { primary: string; secondary: string }> = {};
 	let copied = false;
+	let tags_removed = false;
 	let timer: ReturnType<typeof setTimeout>;
     let can_scroll: boolean;
+	let tagged_text: string = "";
 
 	function set_color_map(): void {
 		// if a label in the color map is not in the value, remove it from the color map
 		for (let label in current_color_map) {
 			if (!value.map(([_, label]) => label).includes(label)) {
 				delete current_color_map[label];
 			}
@@ -59,27 +61,35 @@
 			marked_el_text = value.map(([text, category]) => {
 				if (category !== null) {
 					return `<mark class="hl ${category}" style="background-color:${_color_map[category].secondary}">${text}</mark>`;
 				} else {
 					return text;
 				}
 			}).join("");
+			tagged_text = value.map(([text, category]) => {
+				if (category !== null) {
+					return `<${category}>${text}</${category}>`;
+				} else {
+					return text;
+				}
+			}).join("");
 		}
 	}
 
 	$: set_color_map();
 	$: set_text_from_value(true);
 
 	const dispatch = createEventDispatcher<{
 		change: [string, string | null][];
 		input: [string, string | null][];
 		submit: undefined;
 		blur: undefined;
 		select: SelectData;
 		focus: undefined;
+		clear: undefined;
 	}>();
 
     beforeUpdate(() => {
 		can_scroll = el && el.offsetHeight + el.scrollTop > el.scrollHeight - 100;
 	});
 
 	function handle_change(): void {
@@ -130,27 +140,19 @@
 		}
 		if (text) {
 			new_value.push([text, category]);
 		}
 		value = new_value;
 	}
 
-	async function handle_copy(): Promise<void> {
-		if ("clipboard" in navigator) {
-			await navigator.clipboard.writeText(el_text);
-			copy_feedback();
-		}
-	}
-
-	function copy_feedback(): void {
-		copied = true;
-		if (timer) clearTimeout(timer);
-		timer = setTimeout(() => {
-			copied = false;
-		}, 1000);
+	function handle_remove_tags(): void {
+		marked_el_text = el_text;
+		handle_change();
+		tags_removed = true;
+		dispatch("clear");
 	}
 
 	// Method to remove highlight if cursor is inside
 	function checkAndRemoveHighlight() {
 		const selection = window.getSelection();
 		const cursorPosition = selection.anchorOffset;
 		if (selection.rangeCount > 0) {
@@ -172,88 +174,58 @@
 				newSelection.removeAllRanges();
 				newSelection.addRange(range);
 			}
 		}
 	}
 </script>
 
-<!-- svelte-ignore a11y-no-static-element-interactions -->
-<!-- svelte-ignore a11y-click-events-have-key-events-->
-<label class:container>
+<label class:container for="highlighted-textbox">
 	<BlockTitleWithHighlights {show_label} {show_legend} {show_legend_label} {legend_label} {_color_map} {info}>{label}</BlockTitleWithHighlights>
-	{#if show_copy_button}
-		{#if copied}
-			<button
-				in:fade={{ duration: 300 }}
-				aria-label="Copied"
-				aria-roledescription="Text copied"><Check /></button
-			>
-		{:else}
-			<button
-				on:click={handle_copy}
-				aria-label="Copy"
-				aria-roledescription="Copy text"><Copy /></button
-			>
-		{/if}
-	{/if}
-
+	<Widgets
+		{show_copy_button}
+		show_remove_tags_button={show_remove_tags_button && !tags_removed}
+		value={tagged_text}
+		on:removeTags={handle_remove_tags}
+	/>
     {#if disabled}
         <div 
             class="textfield"
             data-testid="highlighted-textbox"
             contenteditable="false"
             bind:this={el}
             bind:textContent={el_text}
             bind:innerHTML={marked_el_text}
         />
     {:else}
-        <div
-            class="textfield"
-            data-testid="highlighted-textbox"
-            contenteditable="true"
-            bind:this={el}
-            bind:textContent={el_text}
-            bind:innerHTML={marked_el_text}
-            on:blur
-            on:keypress
-            on:select
-            on:scroll
-            on:input={handle_change}
-            on:focus
-            on:change={handle_change}
-        />
+<div
+	class="textfield"
+	data-testid="highlighted-textbox"
+	contenteditable="true"
+	role="textbox"
+	tabindex="0"
+	bind:this={el}
+	bind:textContent={el_text}
+	bind:innerHTML={marked_el_text}
+	on:blur
+	on:keypress
+	on:select
+	on:scroll
+	on:input={handle_change}
+	on:focus
+	on:change={handle_change}
+/>
     {/if}
 </label>
 
 <style>
 	label {
 		display: block;
 		width: 100%;
 	}
 
-	button {
-		display: flex;
-		position: absolute;
-		top: var(--block-label-margin);
-		right: var(--block-label-margin);
-		align-items: center;
-		box-shadow: var(--shadow-drop);
-		border: 1px solid var(--color-border-primary);
-		border-top: none;
-		border-right: none;
-		border-radius: var(--block-label-right-radius);
-		background: var(--block-label-background-fill);
-		padding: 5px;
-		width: 22px;
-		height: 22px;
-		overflow: hidden;
-		color: var(--block-label-color);
-		font: var(--font-sans);
-		font-size: var(--button-small-text-size);
-	}
 	.container {
 		display: flex;
 		flex-direction: column;
 		gap: var(--spacing-sm);
 	}
 
 	.textfield {
```

### Comparing `gradio_highlightedtextbox-0.0.8/frontend/Index.svelte` & `gradio_highlightedtextbox-0.0.9/frontend/Index.svelte`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 	export let gradio: Gradio<{
 		change: never;
 		input: never;
 		submit: never;
 		select: SelectData;
 		focus: never;
 		blur: never;
+		clear: never;
 	}>;
 
 	export let label = "Highlighted Textbox";
 	export let legend_label: string | undefined = "Highlights:";
 	export let info: string | undefined = undefined;
 	export let elem_id = "";
 	export let elem_classes: string[] = [];
@@ -28,14 +29,15 @@
 	export let show_legend: boolean;
 	export let show_legend_label: boolean;
 	export let color_map: Record<string, string> = {};
 	export let container: boolean = true;
 	export let scale: number | null = null;
 	export let min_width: number | undefined = undefined;
 	export let show_copy_button: boolean = false;
+	export let show_remove_tags_button: boolean = false;
 	export let loading_status: LoadingStatus | undefined = undefined;
 	export let value_is_output: boolean = false;
 	export let combine_adjacent: boolean = false;
 	export let interactive: boolean = true;
 	export const autofocus: boolean = false;
 	export const autoscroll: boolean = true;
 
@@ -72,17 +74,19 @@
 		{info}
 		{show_label}
 		{show_legend}
 		{show_legend_label}
 		{legend_label}
 		{color_map}
 		{show_copy_button}
+		{show_remove_tags_button}
 		{container}
 		disabled={!interactive}
 		on:change={() => gradio.dispatch("change")}
 		on:input={() => gradio.dispatch("input")}
 		on:submit={() => gradio.dispatch("submit")}
 		on:blur={() => gradio.dispatch("blur")}
 		on:select={(e) => gradio.dispatch("select", e.detail)}
 		on:focus={() => gradio.dispatch("focus")}
+		on:clear={function (){ console.log("test"); gradio.dispatch("clear");}}
 	/>
 </Block>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 visible} {elem_id} {elem_classes} {scale} {min_width} allow_overflow={false}
 padding={container} > {#if loading_status}
 ...loading_status} /> {/if}
 label} {info} {show_label} {show_legend} {show_legend_label} {legend_label}
-{color_map} {show_copy_button} {container} disabled={!interactive} on:change={
-() => gradio.dispatch("change")} on:input={() => gradio.dispatch("input")} on:
-submit={() => gradio.dispatch("submit")} on:blur={() => gradio.dispatch
-("blur")} on:select={(e) => gradio.dispatch("select", e.detail)} on:focus={()
-=> gradio.dispatch("focus")} />
+{color_map} {show_copy_button} {show_remove_tags_button} {container} disabled=
+{!interactive} on:change={() => gradio.dispatch("change")} on:input={() =>
+gradio.dispatch("input")} on:submit={() => gradio.dispatch("submit")} on:blur={
+() => gradio.dispatch("blur")} on:select={(e) => gradio.dispatch("select",
+e.detail)} on:focus={() => gradio.dispatch("focus")} on:clear={function ()
+{ console.log("test"); gradio.dispatch("clear");}} />
```

### Comparing `gradio_highlightedtextbox-0.0.8/frontend/package-lock.json` & `gradio_highlightedtextbox-0.0.9/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_highlightedtextbox-0.0.8/frontend/utils.ts` & `gradio_highlightedtextbox-0.0.9/frontend/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_highlightedtextbox-0.0.8/README.md` & `gradio_highlightedtextbox-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,40 +47,40 @@
     msg: str,
 ) -> None:
     gr.Info(
         f"{msg}: {HighlightedTextbox.tuples_to_tagged_text(highlighted_text['data'], tag_id, tag_open, tag_close)}"
     )
 
 
-initial_text = "It is not something to be ashamed of: it is no different from the <d>personal fears</d> and <tm>dislikes</tm> of other things that <t>manny peopl</t> have."
+initial_text = "It is not something to be ashamed of: it is no different from the <a>personal fears</a> and <b>dislikes</b> of other things that <c>manny peopl</c> have."
 
 with gr.Blocks() as demo:
     gr.Markdown("### Parameters to control the highlighted textbox:")
     with gr.Row():
         tag_id = gr.Dropdown(
-            choices=["Typo", "Terminology", "Disfluency"],
-            value=["Typo", "Terminology", "Disfluency"],
+            choices=["Error A", "Error B", "Error C"],
+            value=["Error A", "Error B", "Error C"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag ID",
             show_label=True,
             info="Insert one or more tag IDs to use in the highlighted textbox.",
         )
         tag_open = gr.Dropdown(
-            choices=["<t>", "<tm>", "<d>"],
-            value=["<t>", "<tm>", "<d>"],
+            choices=["<a>", "<b>", "<c>"],
+            value=["<a>", "<b>", "<c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag open",
             show_label=True,
             info="Insert one or more tags to mark the beginning of a highlighted section.",
         )
         tag_close = gr.Dropdown(
-            choices=["</t>", "</tm>", "</d>"],
-            value=["</t>", "</tm>", "</d>"],
+            choices=["</a>", "</b>", "</c>"],
+            value=["</a>", "</b>", "</c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag close",
             show_label=True,
             info="Insert one or more tags to mark the end of a highlighted section.",
         )
     gr.Markdown(
@@ -109,14 +109,16 @@
             interactive=True,
             label="Highlighted text",
             info="Textbox containing editable text with custom highlights.",
             show_legend=True,
             show_label=True,
             legend_label="Legend:",
             show_legend_label=True,
+            show_remove_tags_button=True,
+            show_copy_button=False,
         )
 
     # Functions
 
     tagged.input(
         fn=convert_tagged_text_to_highlighted_text,
         inputs=[tagged, tag_id, tag_open, tag_close],
@@ -128,22 +130,22 @@
         outputs=tagged,
     )
     high.focus(
         fn=show_info,
         inputs=[high, tag_id, tag_open, tag_close, gr.State("Focus")],
         outputs=None,
     )
-    high.change(
+    high.blur(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Change")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
         outputs=None,
     )
-    high.blur(
+    high.clear(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Remove tags")],
         outputs=None,
     )
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
@@ -443,27 +445,41 @@
 bool
 ```
 
 </td>
 <td align="left"><code>False</code></td>
 <td align="left">If True, includes a copy button to copy the text in the textbox. Only applies if show_label is True.</td>
 </tr>
+
+<tr>
+<td align="left"><code>show_remove_tags_button</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+bool
+```
+
+</td>
+<td align="left"><code>False</code></td>
+<td align="left">If True, includes a button to remove all tags from the text.</td>
+</tr>
 </tbody></table>
 
 
 ### Events
 
 | name | description |
 |:-----|:------------|
 | `change` | Triggered when the value of the HighlightedTextbox changes either because of user input (e.g. a user types in a textbox) OR because of a function update (e.g. an image receives a value from the output of an event trigger). See `.input()` for a listener that is only triggered by user input. |
 | `input` | This listener is triggered when the user changes the value of the HighlightedTextbox. |
 | `select` | Event listener for when the user selects or deselects the HighlightedTextbox. Uses event data gradio.SelectData to carry `value` referring to the label of the HighlightedTextbox, and `selected` to refer to state of the HighlightedTextbox. See EventData documentation on how to use this event data |
 | `submit` | This listener is triggered when the user presses the Enter key while the HighlightedTextbox is focused. |
 | `focus` | This listener is triggered when the HighlightedTextbox is focused. |
 | `blur` | This listener is triggered when the HighlightedTextbox is unfocused/blurred. |
+| `clear` | This listener is triggered when the user clears the HighlightedTextbox using the X button for the component. |
 
 
 
 ### User function
 
 The impact on the users predict function varies depending on whether the component is used as an input or output for an event (or both).
```

### Comparing `gradio_highlightedtextbox-0.0.8/pyproject.toml` & `gradio_highlightedtextbox-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,18 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_highlightedtextbox"
-version = "0.0.8"
+version = "0.0.9"
 description = "Editable Gradio textarea supporting highlighting"
 readme = "README.md"
-license = "mit"
+license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Gabriele Sarti", email = "gabriele.sarti996@gmail.com" }]
 keywords = ["gradio-custom-component", "gradio-template-SimpleTextbox", "highlight", "textbox", "editing", "color"]
 # Add dependencies here
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
@@ -35,11 +35,11 @@
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [project.urls]
 space = "https://huggingface.co/spaces/gsarti/gradio_highlightedtextbox"
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_highlightedtextbox/templates", "*.pyi", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "Users/gsarti/Documents/projects/highlightedtextbox/backend/gradio_highlightedtextbox/templates", "Users/gsarti/Documents/projects/highlightedtextbox/backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates"]
+artifacts = ["/backend/gradio_highlightedtextbox/templates", "*.pyi", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "Users/gsarti/Documents/projects/highlightedtextbox/backend/gradio_highlightedtextbox/templates", "Users/gsarti/Documents/projects/highlightedtextbox/backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates", "backend/gradio_highlightedtextbox/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_highlightedtextbox"]
```

### Comparing `gradio_highlightedtextbox-0.0.8/PKG-INFO` & `gradio_highlightedtextbox-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_highlightedtextbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Editable Gradio textarea supporting highlighting
 Project-URL: space, https://huggingface.co/spaces/gsarti/gradio_highlightedtextbox
 Author-email: Gabriele Sarti <gabriele.sarti996@gmail.com>
 License-Expression: MIT
 Keywords: color,editing,gradio-custom-component,gradio-template-SimpleTextbox,highlight,textbox
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
@@ -74,40 +74,40 @@
     msg: str,
 ) -> None:
     gr.Info(
         f"{msg}: {HighlightedTextbox.tuples_to_tagged_text(highlighted_text['data'], tag_id, tag_open, tag_close)}"
     )
 
 
-initial_text = "It is not something to be ashamed of: it is no different from the <d>personal fears</d> and <tm>dislikes</tm> of other things that <t>manny peopl</t> have."
+initial_text = "It is not something to be ashamed of: it is no different from the <a>personal fears</a> and <b>dislikes</b> of other things that <c>manny peopl</c> have."
 
 with gr.Blocks() as demo:
     gr.Markdown("### Parameters to control the highlighted textbox:")
     with gr.Row():
         tag_id = gr.Dropdown(
-            choices=["Typo", "Terminology", "Disfluency"],
-            value=["Typo", "Terminology", "Disfluency"],
+            choices=["Error A", "Error B", "Error C"],
+            value=["Error A", "Error B", "Error C"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag ID",
             show_label=True,
             info="Insert one or more tag IDs to use in the highlighted textbox.",
         )
         tag_open = gr.Dropdown(
-            choices=["<t>", "<tm>", "<d>"],
-            value=["<t>", "<tm>", "<d>"],
+            choices=["<a>", "<b>", "<c>"],
+            value=["<a>", "<b>", "<c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag open",
             show_label=True,
             info="Insert one or more tags to mark the beginning of a highlighted section.",
         )
         tag_close = gr.Dropdown(
-            choices=["</t>", "</tm>", "</d>"],
-            value=["</t>", "</tm>", "</d>"],
+            choices=["</a>", "</b>", "</c>"],
+            value=["</a>", "</b>", "</c>"],
             multiselect=True,
             allow_custom_value=True,
             label="Tag close",
             show_label=True,
             info="Insert one or more tags to mark the end of a highlighted section.",
         )
     gr.Markdown(
@@ -136,14 +136,16 @@
             interactive=True,
             label="Highlighted text",
             info="Textbox containing editable text with custom highlights.",
             show_legend=True,
             show_label=True,
             legend_label="Legend:",
             show_legend_label=True,
+            show_remove_tags_button=True,
+            show_copy_button=False,
         )
 
     # Functions
 
     tagged.input(
         fn=convert_tagged_text_to_highlighted_text,
         inputs=[tagged, tag_id, tag_open, tag_close],
@@ -155,22 +157,22 @@
         outputs=tagged,
     )
     high.focus(
         fn=show_info,
         inputs=[high, tag_id, tag_open, tag_close, gr.State("Focus")],
         outputs=None,
     )
-    high.change(
+    high.blur(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Change")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
         outputs=None,
     )
-    high.blur(
+    high.clear(
         fn=show_info,
-        inputs=[high, tag_id, tag_open, tag_close, gr.State("Blur")],
+        inputs=[high, tag_id, tag_open, tag_close, gr.State("Remove tags")],
         outputs=None,
     )
 
 if __name__ == "__main__":
     demo.launch()
 
 ```
@@ -470,27 +472,41 @@
 bool
 ```
 
 </td>
 <td align="left"><code>False</code></td>
 <td align="left">If True, includes a copy button to copy the text in the textbox. Only applies if show_label is True.</td>
 </tr>
+
+<tr>
+<td align="left"><code>show_remove_tags_button</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+bool
+```
+
+</td>
+<td align="left"><code>False</code></td>
+<td align="left">If True, includes a button to remove all tags from the text.</td>
+</tr>
 </tbody></table>
 
 
 ### Events
 
 | name | description |
 |:-----|:------------|
 | `change` | Triggered when the value of the HighlightedTextbox changes either because of user input (e.g. a user types in a textbox) OR because of a function update (e.g. an image receives a value from the output of an event trigger). See `.input()` for a listener that is only triggered by user input. |
 | `input` | This listener is triggered when the user changes the value of the HighlightedTextbox. |
 | `select` | Event listener for when the user selects or deselects the HighlightedTextbox. Uses event data gradio.SelectData to carry `value` referring to the label of the HighlightedTextbox, and `selected` to refer to state of the HighlightedTextbox. See EventData documentation on how to use this event data |
 | `submit` | This listener is triggered when the user presses the Enter key while the HighlightedTextbox is focused. |
 | `focus` | This listener is triggered when the HighlightedTextbox is focused. |
 | `blur` | This listener is triggered when the HighlightedTextbox is unfocused/blurred. |
+| `clear` | This listener is triggered when the user clears the HighlightedTextbox using the X button for the component. |
 
 
 
 ### User function
 
 The impact on the users predict function varies depending on whether the component is used as an input or output for an event (or both).
```

