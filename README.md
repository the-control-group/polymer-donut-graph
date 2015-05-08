# polymer-donut-graph

**This element is compatible with Polymer 0.5.**

__Example:__

```
	<polymer-element name="polymer-donut-graph-demo">
		<template>
			<polymer-donut-graph
				series="{{ series }}"
				innerSize="{{ innerSize }}"
				innerColor="{{ innerColor }}"
				chartTitle="{{ chartTitle }}"></polymer-donut-graph>
		</template>
		<script src="../lodash/lodash.js"></script>
		<script>
			Polymer({
				publish: {
					chartTitle: 'polymer-donut-graph-demo',
					innerSize: '70%',
					innerColor: '#fff',
					series: [{
						group: 'Red',
						color: '#f00',
						data: [
							{
								name: 'Ruby',
								y: 5,
								color: '#600'
							},
							{
								name: 'Rose',
								y: 3,
								color: '#fcc'
							},
							{
								name: 'Defaulting Color',
								y: 2
							}
						]
					}, {
						group: 'Blue',
						color: '#00f',
						data: [
							{
								name: 'Sky',
								y: 5,
								color: '#0cf'
							},
							{
								name: 'Navy',
								y: 3,
								color: '#006'
							}
						]
					}]
				},
			});
		</script>
	</polymer-element></polymer-element>
	<polymer-donut-graph-demo></polymer-donut-graph-demo>
```

### `series`

Array of objects containing name and data points.
```
[{
	group: 'Red',
	color: '#f00',
	data: [
		{
			name: 'Ruby',
			y: 5,
			color: '#600'
		},
		{
			name: 'Rose',
			y: 3,
			color: '#fcc'
		},
		{
			name: 'Defaulting Color',
			y: 2
		}
	]
}, {
	group: 'Blue',
	color: '#00f',
	data: [
		{
			name: 'Sky',
			y: 5,
			color: '#0cf'
		},
		{
			name: 'Navy',
			y: 3,
			color: '#006'
		}
	]
}]
```

### `chartTitle`

Title displayed above graph. Default `null`

### `innerSize`

Size of the inner circle compared to outer circle. Default `'50%'`

### `innerColor`

Color of the inner circle labels