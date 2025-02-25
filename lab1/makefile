AUTOPILOT_ROOT :=/escnfs/home/csesoft/xilinx/2024-vitis-vivado/Vitis_HLS/2024.2

ASSEMBLE_SRC_ROOT := .

IFLAG += -I "${AUTOPILOT_ROOT}/include"
IFLAG += -D__SIM_FPO__ -D__SIM_OPENCV__ -D__SIM_FFT__ -D__SIM_FIR__ -D__SIM_DDS__ -D__DSP48E1__ -DHLS_NO_XIL_FPO_LIB
IFLAG += -g 

CFLAG += -fPIC -O0
CFLAG += -lm
CFLAG += -std=c++11 -Wno-unused-result 

all:
	g++ *.cpp -o result $(CFLAG) $(IFLAG)
	
clean:
	rm -rf *.o result
