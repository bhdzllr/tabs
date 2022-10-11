# Tabs #

Tabs with automatic activation as web component - accessible and styleable.


## Usage ##

Install with

```
npm install @bhdzllr/tabs
```


## Example ##

Import the component in your JS file:

```JavaScript
import { Tabs } from '@bhdzllr/tabs';
```

Example with title and `aria-labelledby`:

```HTML
<h1 id="jl-tablist-title">Justice League Members</h1>

<bhdzllr-tabs aria-labelledby="jl-tablist-title">
	<button slot="tab">Batman</button>
	<button slot="tab">Superman</button>
	<button slot="tab">Wonder Woman</button>
	<button slot="tab">The Flash</button>
	<button slot="tab">Cyborg</button>
	<button slot="tab">Aquaman</button>

	<section slot="tabpanel">
		<h2>Batman</h2>
		<p>Content Batman</p>
	</section>
	<section slot="tabpanel">
		<h2>Superman</h2>
		<p>Content Superman</p>
	</section>
	<section slot="tabpanel">
		<h2>Wonder Woman</h2>
		<p>Content Wonder Woman</p>
	</section>
	<section slot="tabpanel">
		<h2>The Flash</h2>
		<p>Content The Flash</p>
	</section>
	<section slot="tabpanel">
		<h2>Cyborg</h2>
		<p>Content Cyborg</p>
	</section>
	<section slot="tabpanel">
		<h2>Aquaman</h2>
		<p>Content Aquaman</p>
	</section>
</bhdzllr-tabs>
```

Example with `aria-label` on web component.

It's also possible to use the component without CSS or JS for progressive
enhancement. Just add attribute `hidden` to the buttons and in CSS make sure
they are visible with `display: inline-block`. With that you have just
the tab panels without the buttons if JS is disabled and no tab buttons if
styling is disabled.

```HTML
<bhdzllr-tabs wa-aria-label="Justice League Members">
	<button slot="tab" hidden>Batman</button>
	<button slot="tab" hidden>Superman</button>
	<button slot="tab" hidden>Wonder Woman</button>
	<button slot="tab" hidden>Cyborg</button>
	<button slot="tab" hidden>Aquaman</button>

	<section slot="tabpanel">
		<h2>Batman</h2>
		<p>Content Batman</p>
	</section>
	<section slot="tabpanel">
		<h2>Superman</h2>
		<p>Content Superman</p>
	</section>
	<section slot="tabpanel">
		<h2>Wonder Woman</h2>
		<p>Content Wonder Woman</p>
	</section>
	<section slot="tabpanel">
		<h2>The Flash</h2>
		<p>Content The Flash</p>
	</section>
	<section slot="tabpanel">
		<h2>Cyborg</h2>
		<p>Content Cyborg</p>
	</section>
	<section slot="tabpanel">
		<h2>Aquaman</h2>
		<p>Content Aquaman</p>
	</section>
</bhdzllr-tabs>
```
