# Cesium Ion Support Added to osgEarth

[Pelican Mapping](http://web.pelicanmapping.com/) has added support for Cesium Ion to their [osgEarth](https://github.com/gwaldron/osgearth) globe rendering toolkit!

osgEarth is an extension to the [OpenSceneGraph](https://www.openscenegraph.org) scene graph library that brings the power of modern geospatial technology to OpenSceneGraph based applications.  osgEarth powers everything from basic GIS applications to high performance flight simulators and nationwide weather and traffic television broadcasts.

osgEarth supports a wide array of datasources, and now osgEarth users can now access imagery layers in their Cesium Ion account using the new [cesiumion](http://docs.osgearth.org/en/latest/references/drivers/tile/cesiumion.html) driver.

The simplest way to get started with Cesium Ion in osgEarth is to create an Earth file that references your Cesium Ion asset id and provide your API token.  It's as simple as this:

```
<map name="Cesium Ion" type="geocentric" version="2"> 
    
    <image name="bluemarble" driver="cesiumion">
        <asset_id>3845</asset_id>
        <token>YOUR_API_TOKEN</token>
    </image>    
    
</map>
```

You can viewer your map using osgearth_viewer or any other osgEarth based application
```
osgearth_viewer cesiumion.earth
```

