* * *
- **Respond time**:
	- Total time to complete single task
	Example:
	 - Access disk, memory, I/O, OS, v.v...

- Performance: Total work done per unit time
	Example:
	- Tasks/transactions/...per hour
- **Define Performance**
$$Performance= \frac{1}{{Execution \ time}}$$

***
**Quick compare**

| X | | Y 
:--:|:--:|:--:
| Performance | > | Performance 
| 1 | | 1
| ------------ | > | ------------ 
| Execution time X | > | Execution time Y

* * *
#### Relative Performance
"X is n time faster than Y"

$$\frac{{Performance(X)}}{{Performance(Y)}} = \frac{{Execution \ time(Y)}}{{Execution \ time(X)}} = n$$
* * *
#### Clock

- Computer require single clock to identify when 1 instruction initialize inside hardware
	- Block create a temporary unit time for computer to do it which called  block creator
- Two defination about clock:
	- Clock cycle
	- Clock rate or Clock frequency

- Clock cycle and Clock frequency
![[Pasted image 20231203101505.png]]
***
$$Clock \ cycle \ time/ Clock \ cycle / Cycle \ time = 0,5\times10^{-9}$$
***
$$Clock \ rate =\frac{1}{Clock \ Cycle} = \frac{1}{0,5\times10^{-9}} = 2\times10^{9}Hz=2GHz$$
***
$$Execution \ time = Total \ clock \ cycle \times Clock \ Cycle$$

$$Execution \ time = \frac{Total \ clock \ cycle}{Clock \ Rate}$$

To enhance performance, we can reduce clock cycle(increase clock rate)

***
### CPI (Clock cycle Per Instruction)

$$Total \ cycle \ clock = Total \ instruction \times CPI$$

$$Execution \ time=Total \ instruction \times CPI \times Clock \ Cycle $$
$$Execution \ time = \frac{Total \ instruction \times CPI}{Clock \ Rate}$$
Per instruction has multiple different instruction group
$$Clock \ Cycle = \sum_{i=1} ^{n}(CPI(i) \times Instruction(i) )
$$

$$CPI = \frac{Clock \ Cycle}{Total \ instruction} = \sum_{i=1} ^{n}(CPI(i) \times \frac{Instruction(i)}{Total \ instruction})$$
***
### IPC (Instruction per cycle)

$$IPC = \frac{1}{CPI}=\frac{Instruction}{Time \times Clock \ Rate(Total \ cycle)}
$$
* * * 
### Factor impact on performance

Performance components:
- Execution time
- Total instruction
- Frequency
- CPI

  | Hardware/Software | What impact's|
  :--:|:--:
  | Algorithm | Total Instruction, CPI|
  | Programming Language | Total Instruction, CPI
  | Compiler | Total Instruction, CPI
  | Instruction Architecture | Total Instruction, Frequency, CPI
  
***
#### Reduce execution time
- Increase clock rate (limited by hardware)
- Pipeline: execution **multiple instruction** by divide cycle execution into many stage. In single time, 1 instruction just can execute 1 stage.
- Prediction: Predict jump (Jump instruction) has or not
- Multicor: Execution many *program* by increase processor
- Multithread: Execution *multitask* by increase processor unit
- Memory hierarchy: Using flash memory for interact with data, using slow mem for storing data.
* * *

