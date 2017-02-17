# ChartsLab-Axis
The axis component renders human-readable reference marks for [Scale](https://github.com/HishamElamir/ChartsLab-Scale/). This alleviates one of the more tedious tasks in visualizing data.
The axis component also uses html5 canvas element for drawing so it keeps your code beautiful and clean.

## Installing
For now you can download the latest release. You can also load directly from [Site(NotFound)](https://github.com/HishamElamir/), either as standalone micro library or as part of ChartsLab release.
```html
<script src="chartsLab/Axis.js"></script>
<script>
var axis = new Axis(canvasContext);
</script>
```

## Requires
Axis component requires just [Scale](https://github.com/HishamElamir/ChartsLab-Scale/) for ticks optimizing.

## API Reference

Axis rendered at specific oriantation(Side) and position. To change the position of the axis with respect to the chart, just give position function a start position and end(finish) position points. And Side function is the oriantation of the axis ticks and lable, at the end just call draw for render the component at the canvas. For example:

```js
Axis
  .Position([50,50], [500,50])
  .Side("TOP")
  .Draw();
```
The micro library API gives you alot of functionality to manipulate the components type and style and values as easy as possible

![ChartsLab-Axis](/Images/AxisOne.JPG)


<a name="Axis" href="#axis">#</a> d3.<b>Axis</b>(<i>canvasContext</i>)

Constructs a new axis generator object for the given with ready for drawing with defaults
 [Tick number](#TickNumber), [Inner tick number](#InnerTickNumber) is equals to 3, [Tick label padding](#TickLabelPadding)

