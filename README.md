# options-fpga

pricing options using FPGAs

although the code is not on the github as of right now due to us working on it on one computer solely (we only have one fpga)... it is coming soon we promise! this project is being worked on by my friend Nathan and I

**as a general outline of what we are doing here please take a look at the image in the repo which shows the project architecture (image forgets to mention that Verilog is used for FPGA programming)**

we want to utilize the "field programmable" aspect of FPGAs to both price options using MC simulations which can be massively parallelized on the FPGA as well as conduct dynamic delta hedging operations to a constantly updating portfolio

the reasoning behind not simply running this on a CPU or CPU is that the large number of random numbers which are generated can often lead to branch misprediction and cache misses, which are even more dangerous on GPUs which lack branch prediction and prefetchers. thus fpgas are able to solve this through hardware branches and custom loading logic (Barbone et. al.).

here are some of the sources we used for our project: 
 - https://www.youtube.com/watch?v=fzikOtbVEL8
 - https://medium.com/@alexander.tsoskounoglou/pricing-options-with-fourier-series-p3-the-heston-model-d157369a217a
 - https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2943608
 - Professor Jean-Pierre Zigrand @ LSE
 - The FPGA Programming Handbook by Bruno and Eschemann
 - https://indico.cern.ch/event/1170079/attachments/2484554/4269717/Demonstration_of_FPGA_Acceleration_of_MonteCarlo_Simulation%20(1).pdf
