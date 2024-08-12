# options-fpga

pricing options using FPGAs

although the code is not on the github as of right now due to us working on it on one computer solely (we only have one fpga)... it is coming soon we promise! this project is being worked on by my friend Nathan and I

**as a general outline of what we are doing here please take a look at the image in the repo which shows the project architecture (image forgets to mention that Verilog is used for FPGA programming)**

we want to both price options using MC simulations which can be massively parallelized on the FPGA as well as conduct dynamic delta hedging operations to a constantly updating portfolio

here are some of the sources we used for our project: 
 - https://www.youtube.com/watch?v=fzikOtbVEL8
 - https://medium.com/@alexander.tsoskounoglou/pricing-options-with-fourier-series-p3-the-heston-model-d157369a217a
 - https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2943608
 - Professor Jean-Pierre Zigrand @ LSE
 - The FPGA Programming Handbook by Bruno and Eschemann
