# DGGS Abstract Specification Ontology

This ontology describes elements of the discrete Global Grid System (DGGS) Abstract Specification in Semantic Web terms. 

This ontology is expected to be used for the publication of DGGS datasets. The ontology contains a `Grid` class of object which an implementing dataset will need to define multiple instances of. Each `Grid` must contain `Cell` instances which are a specialised form of the [GeoSPARQL ontology](https://www.ogc.org/standards/geosparql) 's `Feature` class. The geometries of the `Cell` instances are GeoSPARQL `Geometry` instances with the geometry areas described in DGGS terms which, becuase of the way DGGS' work, are literal values matching those of the `Cell` identifiers. The `Geometry` instances are also created using URIs, not Blank Nodes, as is often the case with GeoSPARQL data, so the Geometry instances can be referenced independently from the `Cell` s. This is so the geometries can be reused in multiple datasets.

This ontology was created as part of the [Open Geospatial Consortium](https://www.ogc.org/) 's *[Testbed 16](https://portal.ogc.org/files/?artifact_id=91644#DGGS)* activities for DGGS. It was created by [SURROUND Australia Pty Ltd](https://surroundaustralia.com) but is likely to be owned and published by the OGC going foward.


## Test dataset
A first test dataset implementing this ontology that is already available is the *Testbed 16 rHealPix-based Dataset* (TB16Pix) which is online at:

* <https://w3id.org/dggs/tb16pix>

This dataset is the reference dataset for the TB16Pix DGGS, that is the series of `Grid` instances and their contained `Cell` and `Geometry` instances created with the TB16Pix parameters.


## License
The content of this repository are licensed using the [GPL 3.0 license](https://www.gnu.org/licenses/quick-guide-gplv3.html). See the the [LICENSE file](LICENSE) for details


## Contact
**Nicholas J. Car**  
*Data Systems Architect*  
[SURROUND Australia Pty Ltd](https://surroundaustralia.com)  
<nicholas.car@surroundaustralia.com>  
GitHub: [nicholascar](https://github.com/nicholascar)  
ORCID: <https://orcid.org/0000-0002-8742-7730>  