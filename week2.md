# Laporan Interpretasi Hasil
## Analisis Network Pharmacology Senyawa bioaktif Scutellariae Radix-Coptidis Rhizoma terhadap Aterosklerosis

Scutellariae Radix dan Coptidis Rhizoma merupakan kombinasi tanaman obat tradisional Tiongkok yang telah lama digunakan dalam pengobatan Aterosklerosis dalam penyakit inflamasi dan kardiovaskular. Kombinasi kedua tanaman ini diketahui mengandung berbagai senyawa bioaktif, seperti quercetin, wogonin, baicalein, β-sitosterol, dan berberine yang memiliki aktivitas antioksidan, antiinflamasi, serta pengatur metabolisme lipid (Ji et al, 2023). Dalam penelitian ji et al. (2023) dituliskan bahwa senyawa aktif tersebut berpotensi memberikan efek terapeutik terhadap penyakit aterosklerosis yang melibatkan arteri besar dan sedang melalui mekanisme multi-target dan multi-pathway. Oleh karena itu, dilakukan pendekatan network pharmacology antara senyawa aktif, target protein, serta jalur biologis yang terlibat dalam mekanisme terapeutiknya.

Senyawa aktif diidentifikasi dalam literatur pendukung, diolah dengan mengidentifikasi dari PubChem & Swiss Target Prediction, OMIM, membuat irisan antara target senyawa dan target penyakit, serta PPI dikonstruksi dengan STRING dan divisualisasikan melalui Cytoscape. Analisis GO dan KEGG pathway dilakukan terhadap target irisan untuk mengidentifikasi fungsi biologis serta jalur molekuler yang paling berperan dalam mekanisme kerja senyawa aktif.

![Irisan gen target aterosklerosis dan target metabolit.](/irisan.png "Irisan gen target aterosklerosis dan target metabolit.")
**Gambar 1.Irisan gen target aterosklerosis dan target metabolit**

Terdapat 14 gen irisan antara target penyakit aterosklerosis dan target senyawa aktif Scutellariae Radix-Coptidis Rhizoma. Hasil tersebut menunjukkan bahwa senyawa aktif memiliki potensi dalam memodulasi berbagai target molekuler yang berperan dalam patogenesis aterosklerosis. 

| Name  | Score |
| ------------- |:-------------:|
| IL6    | 78   |
| TNF     | 71     |
| INS      | 69     |
| EGFR     | 69     |
| ILIB    | 65     |
| SRC      | 64     |
| CTNNB1     | 64     |
| AKT1      | 62     |
| ALB      | 57     |
| TLR4      | 50     |
| HIF1A      | 49     |
| ESR1      | 49     |
| NFKB1      | 49     |
| EP300      | 48     |
| SIRT1    | 46     |
| JUN      | 45     |
| PPARG      | 44     |
| APOB      | 42     |
| IL10     | 42     |
| RELA      | 40     |

**Tabel 1. Nilai degree dan Score**

Degree menunjukkan jumlah hubungan langsung yang dimiliki suatu protein dengan protein lain dalam jaringan. Semakin tinggi nilai degree, semakin besar pengaruh protein tersebut dalam jaringan interaksi. Dalam tabel yang telah diolah menggunakan cyto Hubba dengan menggunakan metode Degree, lima protein dengan nilai tertinggi adalah IL6, TNF, INS, EGFR, dan IL1B. Protein-protein tersebut diperkirakan berperan sebagai hub gene karena memiliki konektivitas paling tinggi yang berpotensi menjadi regulator utama dalam proses inflamasi, regulasi metabolisme, proliferasi sel, serta respons imun yang berkontribusi terhadap perkembangan aterosklerosis. Oleh karena itu, protein-protein tersebut diperkirakan menjadi target utama yang dimodulasi oleh senyawa aktif Scutellariae Radix-Coptidis Rhizoma.

![This is an alt text.](/image/Markdown-mark.svg "This is a sample image.")
**Gambar 2. Jaringan Protein-Protein Interaction (PPI) dengan STRING**

Jaringan PPI menunjukkan hubungan antara protein hasil irisan yang diprediksi saling berinteraksi dalam mekanisme biologis aterosklerosis. Berdasarkan hasil analisis menggunakan STRING, sebagian besar protein target saling terhubung membentuk jaringan interaksi kompleks. Hubungan tersebut menunjukkan bahwa mekanisme perkembangan aterosklerosis tidak dikendalikan oleh satu protein saja, melainkan melibatkan berbagai protein yang saling mempengaruhi. 

![This is an alt text.](/image/Markdown-mark.svg "This is a sample image.")
**Gambar 3. Visualisasi jaringan interaksi senyawa-target-pathway**

Senyawa aktif bekerja melalui mekanisme multi-target dan multi-pathway, sehingga satu senyawa mampu berinteraksi dengan beberapa protein target sekaligus. Senyawa β-sitosterol, berberine, dan wogonin berinteraksi dengan beberapa target protein yaitu PPARA, FABP1, FABP5, NR1H3, ESR1. Target-target tersebut berhubungan dengan PPAR signaling pathway. Hubungan antara senyawa aktif, target protein, dan jalur biologis tersebut menunjukkan bahwa efek terapeutik kombinasi tanaman ini memungkinkan diperoleh melalui modulasi berbagai proses biologis yang saling berkaitan.

![This is an alt text.](/image/Markdown-mark.svg "This is a sample image.")
![This is an alt text.](/image/Markdown-mark.svg "This is a sample image.")
**Gambar 4. Hasil enrichment analysis Gene Ontology dan KEGG dalam STRING**

Analisis GO kategori Biological Process menunjukkan bahwa target hasil irisan terutama terlibat dalam proses adenylate cyclase-activating adrenergic receptor signaling pathway, adenylate cyclase-activating G protein-coupled receptor signaling pathway, blood circulation, cellular response to chemical stimulus, dan cellular response to lipid. Proses-proses tersebut berkaitan erat dengan mekanisme inflamasi, stres oksidatif, regulasi apoptosis, maupun metabolisme lipid yang diketahui berperan dalam perkembangan aterosklerosis.

Pada kategori Molecular Function, target menunjukkan pengayaan pada fungsi lipid binding, long-chain fatty acid binding, nuclear receptor activity, metal ion binding, dan 3`,5`-cyclic—AMP phosphodiesterase activity. Sementara itu, analisis KEGG pathway menunjukkan bahwa target hasil irisan terutama terlibat dalam PPAR signaling pathway (hsa03320). Jalur ini merupakan regulator utama metabolisme lipid yang mengendalikan transport asam lemak, oksidasi asam lemak, diferensiasi adiposit, dan homeostasis energi. Aktivasi jalur PPAR diperkirakan membantu memperbaiki  metabolisme lipid, meningkatkan transport dan oksidasi asam lemak, serta mengurangi akumulasi lipid yang berkontribusi terhadap pembentukan plak  aterosklerosis. Hail ini memperkuat dugaan bahwa senyawa aktif Scutellariae Radix-Coptidis Rhizoma bekerja melalui mekanisme multi-target dan multi-pathway dalam menghambat perkembangan aterosklerosis.

## Kesimpulan
Hasil analisis network pharmacology menunjukkan bahwa senyawa bioaktif Scutellariae Radix-Coptidis Rhizoma berpotensi memberikan efek terapeutik terhadap aterosklerosis melalui mekanisme multi-target dan multi-pathway. Protein IL6, TNF, INS, EGFR, dan IL1B diperkaran berperan sebagai hub gene utama dalam jaringan PPI. Analisis GO menunjukkan bahwa target utama berperan dalam regulasi respons terhadap lipid, sirkulasi darah, dan pensinyalan reseptor yang berhubungan dengan metabolisme lipid. Selain itu, PPAR signaling pathway juga jalur biologis yang paling dominan berdasarkan analisis KEGG. 

## Referensi 
Ji, L., Song, T., Ge, C., Wu, Q., Ma, L., Chen, X., Chen, T., Chen, Q., Chen, Z., & Chen, W. (2023). Identification of bioactive compounds and potential mechanisms of Scutellariae Radix-Coptidis Rhizoma in the treatment of atherosclerosis by integrating network pharmacology and experimental validation. Biomedicine & Pharmacotherapy, 165, 115210. https://doi.org/10.1016/j.biopha.2023.115210 

## Workflow
![This is an alt text.](/image/Markdown-mark.svg "This is a sample image.")
