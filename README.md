# Hardware-Implementation-of-Error-Correcting-Codes-for-NAND-Flash-Devices
Hardware for Error Correcting Codes for NAND FLash Devices was designed in this project. Based on the memory constraints of the device such as spare area and number of bits in a page (4096 bits), 9 bits for parity and 247 bits for message were used, thus creating a codeword of 256 bits. 

LDPC codes were implemented first to correct 1 bit error. However, it didn't perform well under the given constraints. (check files: LDPC_Encoder_no4cycle_col3.bsv, ldpc.cpp
and LDPC_Decoder_no4cycle_col3.bsv)

Hence, Reed Muller code was implemented. It was able to correct upto 1 bit error. (check files: rm_code_with_comment.cpp, rm_encoder.bsv and rm_decoder.bsv)

Guided by Dr V Kamakoti, Dept of CSE, IIT Madras, India.

Here are the list of references that were used:

1. NPTEL Course by Dr. Andrew Thangaraj
https://www.youtube.com/playlist?list=PL5002EB7306694E7D

2. Introduction to LDPC Codes by Sarah J Johnson
http://sigpromu.org/sarah/SJohnsonLDPCintro.pdf

3. Software for LDPC Codes
This software was developed by one of the key persons involved with the development of irregular LDPC.
https://www.cs.toronto.edu/~radford/ftp/LDPC-2012-02-11/index.html

4. Reed Muller Code (IIT Gandhinagar) 
https://www.youtube.com/watch?v=MVeqgsRdXUo

5. Reed-Muller Error Correcting Code by Ben Cooke
http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.208.440&rep=rep1&type=pdf

6. Cpp code for generating all possible combinations
https://www.geeksforgeeks.org/print-all-possible-combinations-of-r-elements-in-a-given-array-of-size-n/

7. Hamming Codes by James Fiedler
https://orion.math.iastate.edu/linglong/Math690F04/HammingCodes.pdf

8. BCH Codes by Shan-Yuan Ho
http://math.mit.edu/~shor/18.310/BCH.pdf

