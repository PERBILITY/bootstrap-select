# Getting Started

---

## Quick start

Bootstrap-select requires jQuery v1.9.1+ and Bootstrap 5 (which includes Popper.js). Bootstrap's CSS and JS (dropdown component) are necessary. For Bootstrap 5's requirements, see its [official documentation](https://getbootstrap.com/docs/5.3/getting-started/introduction/).

Several quick start options are available:

- [Download the latest release.](https://github.com/snapappointments/bootstrap-select/archive/v1.14.0-beta3.zip)
- Clone the repo: `git clone https://github.com/snapappointments/bootstrap-select.git`
- Install with [npm](https://www.npmjs.com/package/bootstrap-select): `npm install bootstrap-select`
- Install with [yarn](https://yarn.pm/bootstrap-select): `yarn add bootstrap-select`
- Install with [Composer](https://getcomposer.org): `composer require snapappointments/bootstrap-select`
- Install with [NuGet](https://www.nuget.org/packages/bootstrap-select): `Install-Package bootstrap-select`
- Install with [Bower](https://bower.io): `bower install bootstrap-select`
- Install via CDN ([cdnjs](https://cdnjs.com/libraries/bootstrap-select), [jsDelivr](https://www.jsdelivr.com/package/npm/bootstrap-select) or [PageCDN](https://pagecdn.com/lib/bootstrap-select)):

```html
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-select@1.14.0-beta3/dist/css/bootstrap-select.min.css">

<!-- Latest compiled and minified JavaScript -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap-select@1.14.0-beta3/dist/js/bootstrap-select.min.js"></script>

<!-- (Optional) Latest compiled and minified JavaScript translation files -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap-select@1.14.0-beta3/dist/js/i18n/defaults-*.min.js"></script>
```

<div class="bs-docs-example small">
	The CDN is updated after the release is made public, which means that there is a delay between the publishing of a release and its availability on the CDN.
</div>

# Usage

---
<div class="card border-info">
	<div class="card-body">
		This version of bootstrap-select is being updated for Bootstrap 5. By default, bootstrap-select automatically detects the version of Bootstrap being used. However, there are some instances where the version detection won't work. See the [documentation](https://developer.snapappointments.com/bootstrap-select/options/#bootstrap-version) for more information regarding Bootstrap version detection.
	</div>
</div>

### Via `selectpicker` class
Add the `selectpicker` class to your select elements to auto-initialize bootstrap-select.
```html
<select class="selectpicker">
  <option>Mustard</option>
  <option>Ketchup</option>
  <option>Barbecue</option>
</select>
```

### Via JavaScript
```js
// To style only selects with the my-select class
$('.my-select').selectpicker();
```
or
```js
// To style all selects
$('select').selectpicker();
```

If calling bootstrap-select via JavaScript, you will need to wrap your code in a [`.ready()`](https://api.jquery.com/ready/) block or place it at the bottom of the page (after the last instance of bootstrap-select).

```js
$(function () {
	$('select').selectpicker();
});
```
