# Lab 11 - Counters and Dividers

In this lab, we learned how to make clock dividers from two types of counters.

## Rubric

| Item | Description | Value |
| ---- | ----------- | ----- |
| Summary Answers | Your writings about what you learned in this lab. | 25% |
| Question 1 | Your answers to the question | 25% |
| Question 2 | Your answers to the question | 25% |
| Question 3 | Your answers to the question | 25% |

## Names
Araceli Gomez Chavez & Gabriel Kendall

## Summary
In this lab, clock dividers were designed using flip-flop counters to reduce high-frequency signals to more usable rates. The two approaches that were used were a modulo counter and a ripple counter. The modulo counter used D flip flops, adders, and comparison logic to count to a specific value, reset, and toggle an ouput. The ripple counter on the other hand used cascaded T flip flops. Each stage divided the clock by two, this then resulted in a simpler but less flexible design limited to powers of two. 

## Lab Questions

### 1 - Why does the Modulo Counter actually divide clocks by 2 * Count?
A modulo counter divides the clock by 2*count because the output only toggles once each time the counter reaches its max value. The counter must count uo to the set value for each toggle, it takes one full count to go high and another full count to go low. As a result, it takes two counting cycles to produce one full output period. 

### 2 - Why does the ring counter's output go to all 1s on the first clock cycle?
The ring counter's output goes to all 1's on the first clock cycle because it was not properly initialized. Without a preset, the feedback can cause all flip flops to latch a 1 simultaneously. This happens on the first clock pulse and is an invalid state for the counter. 

### 3 - What width of ring counter would you use to get to an output of ~1KHz?
The width of a ring counter that would be used to get an output of about 1Khz is either 16 bits for a modulo counter or 17 bits for a ripple counter. 

