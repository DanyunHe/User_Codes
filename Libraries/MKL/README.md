### Purpose:

Example of using MKL libraries on the cluster. The specific example creates 100X100 random matrix and diagonalizes it.

### Contents:

(1) mkltest.f90: Fortran source code

(2) Makefile: Makefile to compile the source code

(3) mkltest.sbatch: Btach-job submission script to send the job to the queue

### Example Usage:

	source new-modules.sh
	module load intel/15.0.0-fasrc01
	module load intel-mkl/11.0.0.079-fasrc02
	make
	sbatch mkltest.sbatch
    
### Example Output:

```
 Eigen values of h:
           1  -5.91736279207788     
           2  -5.46223057195222     
           3  -5.01402247958550     
           4  -4.92365788088306     
           5  -4.71719532747042     
           6  -4.69243866838809     
           7  -4.45607559880318     
           8  -4.29364637545953     
           9  -4.12012344100932     
          10  -3.99660839084350     
          11  -3.90052226823178     
          12  -3.71366383892892     
          13  -3.64985201185449     
          14  -3.50489948129217     
          15  -3.30921654333793     
          16  -3.27169786321411     
          17  -3.14507547824661     
          18  -3.03706676148507     
          19  -2.84579866168597     
          20  -2.79756765318062     
          21  -2.68113916426457     
          22  -2.58755799369194     
          23  -2.53192479360829     
          24  -2.43358065612823     
          25  -2.34006979874691     
          26  -2.27145298910520     
          27  -2.08927980559696     
          28  -1.99141571158356     
          29  -1.95177272002116     
          30  -1.92367224249942     
          31  -1.83847268232064     
          32  -1.72347578338053     
          33  -1.54673117196043     
          34  -1.47608579889885     
          35  -1.31132505671051     
          36  -1.27246330367573     
          37  -1.21474856659619     
          38  -1.13060024602766     
          39 -0.950541085973594     
          40 -0.836306686507764     
          41 -0.795894603730402     
          42 -0.713159645220947     
          43 -0.623961609228595     
          44 -0.558815858097630     
          45 -0.508520560674373     
          46 -0.260225338939519     
          47 -0.182325979064908     
          48 -0.137888620902847     
          49 -2.620265254443774E-002
          50  2.387625430879298E-002
          51  8.197053710423560E-002
          52  0.232668350072395     
          53  0.266220942340935     
          54  0.346848296133684     
          55  0.512816289685102     
          56  0.557402035516485     
          57  0.705064665525522     
          58  0.713713184068821     
          59  0.774618995139470     
          60  0.985565830643974     
          61   1.01266899451509     
          62   1.20051033231066     
          63   1.32710989718093     
          64   1.36248459991783     
          65   1.54496436278907     
          66   1.55754026410668     
          67   1.65541692638266     
          68   1.73672385064674     
          69   1.91049710979643     
          70   1.97806390572992     
          71   2.14987877800264     
          72   2.19762145220981     
          73   2.27193550284329     
          74   2.32872258984841     
          75   2.48861555806478     
          76   2.57834042084491     
          77   2.65658387066938     
          78   2.74359307695401     
          79   2.83294227989646     
          80   2.90208097823729     
          81   3.00353736655272     
          82   3.11762095187064     
          83   3.20496366758183     
          84   3.22459252218350     
          85   3.35401535313157     
          86   3.51639633982373     
          87   3.57001316909478     
          88   3.80291154479333     
          89   3.86164774154183     
          90   4.02131697171234     
          91   4.14402961649619     
          92   4.23464408787674     
          93   4.40435952469218     
          94   4.61519725570740     
          95   4.68349506719145     
          96   4.80328316503722     
          97   5.00141432508218     
          98   5.18567834116602     
          99   5.19875053092606     
         100   50.0109460873557     
End of program.
```
