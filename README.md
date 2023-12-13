# NearMapDataCollector
This repo provides the sample code to collect aerial image tiles of the City of Melbourne using Nearmap Tile API. This codes in this repo can be used to collect the multi-resolution data for the following paper that is currently "submitted" to an academic journal for possible publication.
"A Comparative Study of Knowledge Transfer Methods for Misaligned Urban Building Labels". The paper is archived at: [https://arxiv.org/abs/2303.09064](https://arxiv.org/abs/2311.03867)

Please use the Jupyter notebook "Data_gather_from_NearmapTileAPI" to prepare the multi-resolution Teacher's dataset. Similarly, use "student_data_from_orthorectified_image" notebook to prepare image tiles from ortho images. You will need a Nearmap Tile API key to access the image tiles from Nearmap. The orthophotos can be downloaded from their MapBrowser tool. Please visit their website for the details and documentation.

Building samples of the City of Melbourne are available in the CityPolygon folder as "polygons_edited.shp", which is openly available at https://data.melbourne.vic.gov.au/explore/dataset/2020-building-footprints/information/

Building samples of the CBD area of the City of  Melbourne are available in the CityPolygon folder as "Buildings_MelbCBD_100m_buffer.shp".

The manually prepared building labels for the Student's data are not openly available (until 13 Dec 2023). The authors are working on releasing these labels once the permission is granted by the image provider (Nearmap).

The paper is currently under review in a well-reputed journal. The codes for domain adaptation, knowledge distillation, and deep mutual learning will be available in this repo after the paper is published.

If you use the codes from the repo, we appreciate your citation to the paper as:

```json
@misc{neupane2023comparative,
      title={A Comparative Study of Knowledge Transfer Methods for Misaligned Urban Building Labels}, 
      author={Bipul Neupane and Jagannath Aryal and Abbas Rajabifard},
      year={2023},
      eprint={2311.03867},
      archivePrefix={arXiv},
      primaryClass={cs.CV}
}
```
Acknowledgement:
The authors would like to thank Nearmap for providing the API service to collect the image data for the experiments.
