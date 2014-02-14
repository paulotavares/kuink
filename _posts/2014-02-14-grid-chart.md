---
layout: page
title: "Grid - Chart"
category: crtl
date: 2014-02-14 15:01:28
---

Displaying charts

``
<Grid name="absenceCountChart" title="absenceCount" subtitle="justified_vs_unjustified" position="right" pivot="true" pivotlines="id" pivotcols="code" pivotdata="is_unjustified,is_justified" view="chart_v2">
        <View>
            <Param name="yAxisTitle">absence_count</Param>
            <Param name="xAxisTitle">subjects</Param>
            <Param name="type">column</Param>
            <Param name="stacked">false</Param>
        </View>
</Grid>
``
