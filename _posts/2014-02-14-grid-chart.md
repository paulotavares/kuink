---
layout: page
title: "Grid - Chart"
category: ctrl
date: 2014-02-14 15:01:28
---

A chart is a special way to display data. In framework, this is distinguished by view param, in control tag.

The databind must be organized to be transposed. Example:

| id     | category      | count |
| -------|:-------------:| -----:|
| 1      | Bananas       | 23    |
| 2      | Oranges       | 34    |
| 3      | Apples        | 12    |

In this case, the pivotLines are only the id field. 
The pivotcols are only the category and pivotdata is the count field. Like this

```xml
<Grid [...] pivot="true" pivotlines="id" pivotcols="category" pivotdata="count" [...] >
```


Full Code Example


```xml
<Grid name="[name]" title="[title]" subtitle="[subtitle]" position="[position]" pivot="true" pivotlines="[id]" pivotcols="[X axis column]" pivotdata="[series columns separated by comma]" view="chart_v2">
        <View>
            <Param name="yAxisTitle">[vertical axis title]</Param>
            <Param name="xAxisTitle">[horizontal axis title]</Param>
            <Param name="type">[chart type]</Param>
            <Param name="stacked">[true or false]</Param>
        </View>
</Grid>
```
