# Vectortiles Design for Narok water, Kenya

## 1. List of Layers

|Layer|Geometry Type|Min Zoom|Max Zoom|Remarks|
|---|---|---|---|---|
|pipeline|LineString|10|16|It includes all the types of pipeline, but you may seperate by type of pipe such as main line or secondary line if necessary.|
|meter|Point|16|16|It only includes household connections.|
|flowmeter|Point|14|16|It only includes flow meters to cover wider range of zoom level than consumer meters.|
|valve|Point|15|16|eg. gate valve, sluice valve, air valve, non-return valve, etc.|
|firehydrant|Point|15|16|It's firehydrant layer|
|washout|Point|15|16|It's washout layer|
|tank|Polygon|13|16|Distribution tank layer as `Polygon`. However, you might need to change geometry type to `Point`|
|plant|Polygon|10|16|It incudes boundries of Water Treatment Plant and Water Intake|
|parcels|Polygon|16|16|It is polygon of parcels data which was provided by Narok town planning office.|
|parcels_annotation|Point|16|16|We seperated parcel number from other parcel data due to reducing the size of data.|
|village|Polygon|10|16|Narok water is zoning some area which is called `village`, you may change layer name for your company.|
|dma|Polygon|13|16|District Metered Area(DMA) for Non-Revenue Water Management|
|point_annotation|Point|10|16|We put all the annotation data here if we need to show some label.|

In Narok water, although we have a pumping station at the WTP, we don't have layer for pump. I know it is significant for a water company. So, you may need to add a layer for pumping station.