# stsmapgen

The map generator inspired by [Slay the Spire](https://store.steampowered.com/app/646570).

![](https://user-images.githubusercontent.com/59264002/75630736-89e6a080-5c30-11ea-86ed-3f00e3631e48.gif)

## Theory

1. Set start point and end point.
2. Prepare points with Poisson disk sampling.
3. Generate links with Delaunay triangulation.
4. Find the path from the start point to the end point with A*.
5. Exclude random points on the path.
6. Repeat steps 4 and 5 several times.
7. Complete!

## License

stsmapgen is licensed under the MIT license. See the [LICENSE](https://github.com/yurkth/stsmapgen/blob/master/LICENSE) for more information.

Libraries:

- [poisson-disk-sampling](https://github.com/kchapelier/poisson-disk-sampling) from [kchapelier](https://github.com/kchapelier) is licensed under the MIT license.
- [Delaunator](https://github.com/mapbox/delaunator.git) from [mapbox](https://github.com/mapbox) is licensed under the ISC license.
- [ngraph.path](https://github.com/anvaka/ngraph.path) from [anvaka](https://github.com/anvaka) is licensed under the MIT license.
- [ngraph.graph](https://github.com/anvaka/ngraph.graph) from [anvaka](https://github.com/anvaka) is licensed under the BSD 3-Clause license.