# DEREP-NP-PUB-v2
If you use this database, please cite the manuscript DOI: 10.1021/acs.jnatprod.6b01093

Quick Tips to Use the Database in DataWarrior
1)	When you open the DataWarrior file you downloaded, close all graphics windows and leave only the Table and Structures windows open.
2)	 Delete all search criteria on the right pane, if any.
3)	In the EDIT menu select NEW FILTER. Use text filters and the appropriate options in the dropdown box (starts with, contains, equals). To search ranges, use the SLIDER filter format when selecting the new filter and then in the right pane select the min and max values by double-clicking on the numbers at the ends of the slider.
4)	If you could deduce a partial structure from the NMR data, include it in the search: In the EDIT menu select NEW FILTER and then Structure [Structure List, SSS]. On the filters pane, right click in the white part of the filter and choose ADD and draw the substructure. Note that when you hover over an atom a blue dot appears and if click Q, you can define various atom properties. If you draw two substructures in the same filter it will work as OR Boolean. To create an AND query, you need set two Structure [Structure List, SSS] filters. To do this, create a new filter and select SHOW DUPLICATE FILTERS check box. Now, both SS must be present in the same structure. Note, however, that using this procedure you are not counting number of the SS, just their presence.
5)	The yin-yang bouton in each search means a NOT Boolean and can be used to omit structures that comply to the query. 
6)	For other functionalities read DataWarrior help.



Modifications in v2
Date	Issue	status	Req/Sugg_by
17/Jul/17	UNPD InChI and InChIKeys substituted using INDIGO2 InChi Node (KNIME)	Done	Prof. John Blunt
17/Jul/17	8541 duplicated structures (using DW)	removed	Zani
14/Jul/17	Manually correct 40 structures with wrong charges	Done	Zani
14/Jul/17	Included Indigo2 Standardizer node to correct wrong charges	Done	Zani
5/Jul/17	Cq sp in DEREP is not giving the correct counts. It is currently including a terminal alkyne as 2	Fixed	Prof. John Blunt
5/Jul/17	Cq sp is missing CN and C=C=C	Fixed	Prof. John Blunt
5/Jul/17	it would be more logical to have CH3 singlet as arising from CH3-C to be consistent with CH3 doublet and triplet. The count of CH3 All - CH3 singlet would reveal other CH3s on O or N or S.	Fixed	Prof. John Blunt
5/Jul/17	There is currently no count of acetyl groups on N - quite a common feature. Count of amides would also be very useful.	Included	Prof. John Blunt
5/Jul/17	it is very useful to have counts of 1,1 and 1,2 disub alkenes, trisub alkenes and vinyl groups. Another useful count is fully substituted benzenes	Included	Prof. John Blunt
Jun17	CH-O(all) is counting CH anomeric (O-CH-O) twice 	Fixed	Prof. A. Carroll
