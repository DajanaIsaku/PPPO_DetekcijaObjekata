# PPPO_DetekcijaObjekata
Projektni zadatak iz predmeta principi prezentacije i prepoznavanja oblika

Tema projektnog zadatka: Detekcija objekata (broda)

Cilj projekta je razviti model za detekciju i klasifikaciju brodova na fotografijama snimljenim iz ptičje perspektive. Glavni zadatak je predviđanje lokacije broda na svakoj slici, a ove informacije mogu doprineti praćenju brodova iz vazduha. Dataset koji će se koristiti za ovaj projekat sastoji se od slika koje su označene sa ili bez prisustva brodova, kao i sa jednim ili više brodova na slici, različito raspoređenih.

Dataset koji je korišćen u izradi ovog projektnog zadatka nalazi se na sledećoj lokaciji: https://drive.google.com/file/d/1VHbj77uYVjcEh9_e4Y6wgpIMI-8Q2YBo/view?usp=sharing.

Struktura dataset-a:

train_v2 folder: Ovaj folder sadrži slike koje će biti korišćene za treniranje modela. Ukupno, dataset ima 44,533 slike.

test_v2 folder: Sadrži slike koje će se koristiti za testiranje modela. Cilj je detektovati prisustvo brodova na ovim slikama. U ovom folderu se nalazi 6,872 slike.

train_ship_segmentations_v2.csv: CSV fajl koji sadrži podatke za obuku. Sastoji se od dve kolone: "ImageId" koja identifikuje jedinstveni ID slike, i "EncodedPixels" koja sadrži informacije o segmentaciji brodova.

sample_submission_v2.csv: Primer formata fajla koji se očekuje kao rešenje zadatka. Ovaj fajl služi kao referenca za format u kojem treba dostaviti predviđanja.

Realizacija zadatka zahteva razvoj modela za detekciju objekata na slikama, sa posebnim fokusom na brodove. Kao ulaz koristiće se slike iz train_v2 foldera, dok će se performanse modela evaluirati na test_v2 slikama. Rezultati će biti predstavljeni u formatu sličnom sample_submission_v2.csv.

Projekat ima praktičnu primenu u praćenju i analizi brodova iz vazduha, pružajući korisne informacije o njihovom položaju.
