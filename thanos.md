---
layout: page
title: ThanOS RTOS
---

## ThanOS
This project involved the creation of a custom Send-Receive-Reply based Real Time Operating System designed for the STM32F4 to interface with a UART console and train set.
The system was named ThanOS (Thanos from the Avenger movies) since during development bugs were found where GCC inserted assembly instruction muddling callee saved registers that were caused by adding inline assembly. This project is one of my favourites as I got a chance to explore why FreeRTOS (and other RTOS's for that matter) made API and implementation decisions they did.

#### Features and Completed work
-	Developed UART and timing servers for the RTOS to enable communication with a train set and terminal console
-	Validated functionality of RTOS by writing simple programs that interface with all servers
-	Troubleshot bugs in assembly when GCC inadvertently modified user-mode registers

#### Future work
 - Redesign: This was created for a 4th year course and could use touch up from knowledge I've gained since: the kernel-entry and exit could be made more efficient
 - FreeRTOS equivalent? : It would be a challenging and fun project to make a feature complete RTOS for the sake of better understanding
