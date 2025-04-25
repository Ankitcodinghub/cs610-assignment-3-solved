# cs610-assignment-3-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/cs610-general-policies-solved-10/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;128652&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS610 Assignment 3 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
<div class="kksr-stars">
    
<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
    
<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>
                

<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
• You should do this assignment alone.

• Do not copy or turn in solutions from other sources. You will be penalized if caught.

• You can tweak the compilation commands in the Makefile to suit your compiler version and the target architecture.

Submission

• Submission will be through Canvas.

• Submit a compressed file called “⟨roll⟩-assign3.tar.gz”. The compressed file should have the following structure.

— roll

— — roll-assign3.pdf

— — &lt;problem1-dir&gt;

— — — &lt;source-files&gt; — — &lt;problem2-dir&gt;

— — — &lt;source-files&gt; — — &lt;problem3-dir&gt;

— — — &lt;source-files&gt; — — &lt;problem4-dir&gt;

— — — &lt;source-files&gt;

The PDF file should contain descriptions for the first two problems, and your solution for the last problem.

• We encourage you to use the LATEX typesetting system for generating the PDF file. You can use tools like Tikz, Inkscape, or Draw.io for drawing figures if required. You can alternatively upload a scanned copy of a handwritten solution, but make sure the submission is legible.

• You will get up to two late days to submit your assignment, with a 25% penalty for each day.

Evaluation

• Write your programs such that the exact output format (if any) is respected.

• We will evaluate your implementations on a Unix-like system, for example, recent Debianbased distributions installed on KD first floor labs.

• We will evaluate the implementations with our own inputs and test cases, so remember to test thoroughly.

1

Implement matrix-matrix multiplication using (i) SSE4 and (ii) AVX2 intrinsics. Implement an aligned variant and an unaligned variant for each SIMD extension (if available).

Ensure correctness of your result and compare performance across versions. You can assume the data type of a matrix element is single-precision floating-point and the dimensions are a multiple of four.

You can optionally implement optimizations like blocking as an additional variant.

Refer to https://www.intel.com/content/www/us/en/docs/intrinsics-guide/index.html#

for documentation on Intel Intrinsics.

Implement an inclusive prefix sum function using AVX2 instrinsics. Compare the performance with the sequential, OpenMP, and SSE4 versions (discussed in class).

Implement Problem 2 from Assignment 2 using OpenMP (e.g., do not use pthread_create()). Use only OpenMP constructs for synchronization between producers and consumers and also for maintaining the shared buffer. You can continue to make use of Pthread APIs (e.g., condvars) ONLY for cases which cannot covered by OpenMP.

I suggest you do the following before attempting to solve the problem: (i) Fix your Pthreads implementation, if required, and (ii) go through the rest of the OpenMP slides for possible ideas.

Compile the reference code with gcc -O3 -std=c17 -D_POSIX_C_SOURCE=199309L prob4-v0.c -o prob4-v0.out. You are allowed to switch to C++ for your solutions. Submit two files for this problem: roll-no-prob4-v1.c[pp] and roll-no-prob4-v2.c[pp], corresponding to the two parts.

2
