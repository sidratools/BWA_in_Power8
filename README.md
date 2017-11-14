# Porting and Benchmarking of BWAKIT pipeline on Open POWER architecture


## About BWAKIT 
The BWAKIT provides pre-compiled binaries for x86_64 architecture and end-to-end solution for genome mapping. This GitHub repository describes: 
  	
		(a) how to port various pre-built application binaries used in BWAKIT into OpenPOWER architecture 
    	(b) how to execute the BWAKIT pipeline and 
    	(c) how to validate the output results on OpenPOWER to confirm the successful porting of BWAKIT. 


## List of genome application/tools used

	1. BWAKIT (version 0.7.15) https://github.com/lh3/bwa/tree/master/bwakit
	2. Seqtk (version 1.2) https://github.com/lh3/seqtk
	3. Samtools (version 1.3) http://www.htslib.org
	4. Trimadap (version 0.1) https://github.com/lh3/trimadap 
	5. Samblaster (version 0.1.23) https://github.com/GregoryFaust/samblaster
	6. K8 (version 0.2.3-r67) https://github.com/attractivechaos/k8
	7. V8 (version 3.14.5.9) https://github.com/v8/v8
	8. BWA (version 0.7.15) https://github.com/lh3/bwa
	
### Modified source codes and patches for BWAKIT porting (verion 0.1)

	1. ksw-bwa.c 
	2. ksw-trimadap.c 
	3. vec128int.h
		wget --no-check-certificatehttps://www.ibm.com/developerworks/community/files/form/anonymous/api/library/b8b3a7b1-379f-4140-9d5f-73f658d8b2f5/document/79b19df7-a672-4908-920a-8505c2f09d68/version/61956e94-966c-49c9-bfb4-177168cf6b18/media/veclib.1.0.2.tar
		tar xvf veclib.1.0.2.tar 
		cp veclib.1.0.2/include/vec128int.h 
	4. k8_patch 


