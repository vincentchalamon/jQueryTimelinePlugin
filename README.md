# jQueryTimePlugin

[![SensioLabsInsight](https://insight.sensiolabs.com/projects/bfdcdcfa-01c7-4625-9ef9-ceedfcfe8017/mini.png)](https://insight.sensiolabs.com/projects/bfdcdcfa-01c7-4625-9ef9-ceedfcfe8017)

This jQuery plugin allows you to create a timeline.

<img src="http://www.vincent-chalamon.fr/uploads/jquery-timeline.png" />

# How to use

This plugin requires [jQuery 1.8+](http://jquery.com/) :
```html
<script type="text/javascript" src="http://code.jquery.com/jquery-1.10.1.min.js"></script>
<script type="text/javascript" src="path/to/jquery.timeline.js"></script>
<link type="text/css" rel="stylesheet" media="screen" href="path/to/timeline.css" />
```

Now you can use jQuery timeline plugin as following :
```javascript
$(function () {
    $('#timeline').timeline({
        elements: [
            {
                start: '2006-09-01',
                end: '2008-08-31',
                css: 'jquery-timeline-item-formation',
                label: 'DUT Services et Réseaux de Communication'
            },                 {
                start: '2007-03-12',
                end: '2007-04-14',
                label: 'Wacan Communication'
            },                 {
                start: '2007-07-01',
                end: '2007-07-31',
                label: 'Nice Matin'
            },                 {
                start: '2008-04-14',
                end: '2008-07-31',
                label: 'AureXus'
            },                 {
                start: '2008-09-01',
                end: '2011-12-31',
                label: 'EP Factory'
            },                 {
                start: '2008-09-01',
                end: '2009-08-31',
                css: 'jquery-timeline-item-formation',
                label: 'Licence professionnelle Développement Informatique Multi-supports'
            },                 {
                start: '2012-01-01',
                end: '2012-11-30',
                label: 'PL Com'
            },                 {
                start: '2012-12-01',
                end: '2013-03-31',
                label: 'Mayflower'
            },                 {
                start: '2013-04-01',
                label: 'Ylly'
            }
        ],
        onSelect: function(event, index){
            // Do some stuff
        }
    });
});
```

# Options

You must set following options to timeline :

* elements : array of elements to create
    * start : element start date (string or Date object)
    * end : optional element end date (string or Date object)
    * label : element label
    * css : optional element additional class name
* onSelect : callback on click on item
