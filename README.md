## Bootstrap classes

Get familiar with Bootstrap CSS classes:

- utilities classes (`.text-center`, `.list-inline`, etc..)
- UI components classes (`.btn-primary`, `.form-inline`, etc..)


Integrate all these Bootstrap classes on `index.html` page


## Responsive grid

Improve your page using Bootstrap grid to get [this final result](http://lewagon.github.io/bootstrap-challenges/04-bootstrap-mockup-v2/).

- Alway start coding your grid **without content**, and insert your content in the `.col` **as a second step**.

```html
<!-- Example of pure grid code without content -->
<div class="container">
  <div class="row">
    <div class="col-xs-12 col-sm-6"></div>
    <div class="col-xs-12 col-sm-6"></div>
    <div class="col-xs-12 col-sm-6"></div>
    <div class="col-xs-12 col-sm-6"></div>
  </div>
</div>
```

## Tips: map

- For the map section, the code is a bit complicated since it uses a bit of javascript. Here it is:

```html
<div id="map" style="width: 100%; height: 400px;"></div>

<script type="text/javascript" src="https://maps.googleapis.com/maps/api/js"></script>

<script type="text/javascript">
var myLatlng = new google.maps.LatLng(48.852937,2.364178);

var myOptions = {
  zoom: 16,
  center: myLatlng,
  scrollwheel: false,
  mapTypeId: google.maps.MapTypeId.ROADMAP,
  styles: [] // TODO: replace [] by array from https://snazzymaps.com/
};

var map = new google.maps.Map(document.getElementById('map'), myOptions);
var marker = new google.maps.Marker({
  position: myLatlng,
  map: map,
  title: "You are here!"
});
</script>
```

You can pick a nice map theme on [Snazzy Maps](https://snazzymaps.com/) and replace the `[]` in the code above by the JavaScript Style Array you will copy on Snazzyp Maps.
