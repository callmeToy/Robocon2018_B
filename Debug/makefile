################################################################################
# Automatically-generated file. Do not edit!
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include mbed/TARGET_LPC1768/TOOLCHAIN_GCC_CR/subdir.mk
-include Move/subdir.mk
-include subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(CC_DEPS)),)
-include $(CC_DEPS)
endif
ifneq ($(strip $(C++_DEPS)),)
-include $(C++_DEPS)
endif
ifneq ($(strip $(C_UPPER_DEPS)),)
-include $(C_UPPER_DEPS)
endif
ifneq ($(strip $(CXX_DEPS)),)
-include $(CXX_DEPS)
endif
ifneq ($(strip $(CPP_DEPS)),)
-include $(CPP_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

# Add inputs and outputs from these tool invocations to the build variables 

# All Target
all: Robocon2018_B.axf

# Tool invocations
Robocon2018_B.axf: $(OBJS) $(USER_OBJS)
	@echo 'Building target: $@'
	@echo 'Invoking: MCU C++ Linker'
	arm-none-eabi-c++ -nostdlib -L"C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B" -L"C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B\mbed" -L"C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B\mbed\TARGET_LPC1768" -L"C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B\mbed\TARGET_LPC1768\TARGET_NXP" -L"C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B\mbed\TARGET_LPC1768\TARGET_NXP\TARGET_LPC176X" -L"C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B\mbed\TARGET_LPC1768\TARGET_NXP\TARGET_LPC176X\TARGET_MBED_LPC1768" -L"C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B\mbed\TARGET_LPC1768\TOOLCHAIN_GCC_CR" -Xlinker -Map="Robocon2018_B.map" -Xlinker --gc-sections -mcpu=cortex-m3 -mthumb -T "C:\Users\Mayoi\Documents\MCUXpressoIDE_10.1.0_589\workspace\Robocon2018_B\mbed\TARGET_LPC1768\TOOLCHAIN_GCC_CR\LPC1768.ld" -o "Robocon2018_B.axf" $(OBJS) $(USER_OBJS) $(LIBS)
	@echo 'Finished building target: $@'
	@echo ' '
	$(MAKE) --no-print-directory post-build

# Other Targets
clean:
	-$(RM) $(CC_DEPS)$(C++_DEPS)$(EXECUTABLES)$(C_UPPER_DEPS)$(CXX_DEPS)$(OBJS)$(CPP_DEPS)$(C_DEPS) Robocon2018_B.axf
	-@echo ' '

post-build:
	-@echo 'Performing post-build steps'
	-arm-none-eabi-size "Robocon2018_B.axf"; arm-none-eabi-objcopy -O binary "Robocon2018_B.axf" "Robocon2018_B.bin" ; # checksum -p LPC1768 -d "Robocon2018_B.bin";
	-@echo ' '

.PHONY: all clean dependents
.SECONDARY: post-build

-include ../makefile.targets
