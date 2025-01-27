# Project-Vison

Dall’official github siamo riusciti a creare un notebook su Colab VITON-HD_implementation.ipynb, che fa girare tutto il codice contenuto nel https://github.com/shadow2496/VITON-HD (si riesce a fare testing, ma solo con le loro immagini già preprocessate). 

Ma mancano modelli e implementazione del preprocessing, le cui linee guida sono contenute in https://github.com/sangyun884/HR-VITON/blob/main/Preprocessing.md.

L’idea è quella di unire questo codice con quello scritto dall’utente del primo link https://github.com/SwayamInSync/clothes-virtual-try-on. 
In particolare implementare nel colab condiviso VITON-HD_implementation.ipynb le seguenti parti:
Openpose → modello per Pose Estimation
Human parse → creazione di parse map (parti del corpo della figura umana rappresentata, con colori diversi) tramite human segmentation
Densepose → modello per un miglior riconoscimento dei volumi e delle posizioni 3D rispetto a Openpose
Cloth mask → già implementata con metodi OpenCV, per estrazione mask binaria abiti
Parse agnostic → Si riferisce a una rappresentazione semplificata dell'immagine di una persona che rimuove i dettagli riguardanti i vestiti che sta indossando.



Il nostro progetto potrebbe essere quello di ricomporre l’implementazione completa del paper VITON-HD, e una volta capita la pipeline, importare diversi modelli e testarli con metriche per capirne i punti di forza e non.



Pose estimation

https://github.com/ZheC/tf-pose-estimation/tree/master (implementazione di OpenPose alleggerita)

https://colab.research.google.com/drive/1yM--K03ZvSiEi8Pudj5Vj_pWiZ6GI__y#scrollTo=nyoyNJ_GHe76
(colab human pose estimation - openpose)

https://colab.research.google.com/drive/1xVOCyLcUvd8LI7zAnJZUJkZJumqWjDcR?authuser=1#scrollTo=7du-Sgqcl3zi (implementazione VITON-HD)
