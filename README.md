<!DOCTYPE html>

<head>
	<title>Mítika AR</title>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1">

	<link rel="stylesheet" href="demo-styles.css">

	<!-- The following libraries and polyfills are recommended to maximize browser support -->
	<!-- NOTE: you must adjust the paths as appropriate for your project -->

	<!-- 🚨 REQUIRED: Web Components polyfill to support Edge and Firefox < 63 -->
	<script src="https://unpkg.com/@webcomponents/webcomponentsjs@2.1.3/webcomponents-loader.js"></script>

	<!-- 💁 OPTIONAL: Intersection Observer polyfill for better performance in Safari and IE11 -->
	<script src="https://unpkg.com/intersection-observer@0.5.1/intersection-observer.js"></script>

	<!-- 💁 OPTIONAL: Resize Observer polyfill improves resize behavior in non-Chrome browsers -->
	<script src="https://unpkg.com/resize-observer-polyfill@1.5.0/dist/ResizeObserver.js"></script>

	<!-- 💁 OPTIONAL: Fullscreen polyfill is needed to fully support AR features -->
	<script src="https://unpkg.com/fullscreen-polyfill@1.0.2/dist/fullscreen.polyfill.js"></script>

	<!-- 💁 OPTIONAL: Include prismatic.js for Magic Leap support -->
	<script src="https://unpkg.com/@magicleap/prismatic/prismatic.min.js"></script>

	<!-- 💁 OPTIONAL: The :focus-visible polyfill removes the focus ring for some input types -->
	<script src="https://unpkg.com/focus-visible@5.0.2/dist/focus-visible.js" defer></script>

	<!-- Loads <model-viewer> for modern browsers: -->
	<script type="module" src="https://unpkg.com/@google/model-viewer@v0.9.0/dist/model-viewer.js">
	</script>

	<!-- Loads <model-viewer> for old browsers like IE11: -->
	<script nomodule src="https://unpkg.com/@google/model-viewer@v0.9.0/dist/model-viewer-legacy.js">
	</script>

</head>

<body>
	<div id="card">
		<!-- All you need to put beautiful, interactive 3D content on your site: -->
		<model-viewer	src="assets/Astrounaut.glb"
						ios-src="assets/MitikaLogo.usdz"
						alt="Logo da Mítika em 3D"
						shadow-intensity="1"
						camera-controls
						interaction-prompt="auto"
						ar ar-modes="webxr scene-viewer quick-look fallback"
						ar-scale="auto"
						auto-rotate ar magic-leap>
		</model-viewer>
	</div>
</body>

</html>
