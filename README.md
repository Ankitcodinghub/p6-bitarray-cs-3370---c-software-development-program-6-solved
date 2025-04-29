# p6-bitarray-cs-3370---c-software-development-program-6-solved
**TO GET THIS SOLUTION VISIT:** [P6-BitArray CS 3370 – C++ Software Development Program 6 Solved](https://www.ankitcodinghub.com/product/p6-bitarray-cs-3370-c-software-development-program-6-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;60016&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;P6-BitArray  CS 3370 – C++ Software Development  Program 6 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
            5/5 - (1 vote)    </div>
    </div>
“Dynamic Bit Strings”

This assignment uses bitwise operations and operator overloading. You will let the <strong>vector</strong> class template do all of the memory management for you, however (whew!). Users look upon instances of this class as bit strings, indexed left-to-right like any other type of string.&nbsp;&nbsp; Do not think of these as large numbers.

Create a class named <strong>BitArray</strong> that holds a dynamic number of bits, packed into unsigned integers to save space.&nbsp;&nbsp; You will use a vector of integers to store the bits.&nbsp; It is up to you to process bits in the correct position inside the appropriate integer in the vector.

You need to keep track of how many integers are needed to hold the bits in use.&nbsp; As bits are appended, you will have to expand to the vector if it is full (i.e., if all bits are currently used; vector::resize and/or vector::push_back are handy for this).&nbsp; In addition to providing the capability to set, reset, and test individual bits, this class provides some convenient operations commonly needed in bit-related applications.

Remember, the bits appear to the user as if they are bit <em>strings</em>, not numbers, so if the BitArray <strong>b</strong> holds 1011, then the 0<sup>th</sup>, 2<sup>nd</sup>, and 3<sup>rd</sup> bits are 1 and <strong>b[1]</strong> is 0.

We will make the underlying integer type of the array a template parameter, which defaults to <strong>size_t</strong>, so your class definition will look like this:

On most platforms, this means that you can hold 32 or 64 bits in each array element (I’ll call the individual integers “blocks”), but don’t hard code 32 or 64 throughout your code. Instead, you can calculate the number of bits per block at compile time inside your class as follows:

The macro CHAR_BIT is defined in <strong>&lt;climits&gt;</strong>, and is the number 8 on most platforms (duh).

The most efficient way to store bits in each integer may surprise you.&nbsp; To better understand the layout of a <strong>BitArray</strong>, suppose a <strong>BitArray </strong>object currently tracks 84 bits and <strong>sizeof(size_t)</strong> == 4 bytes.&nbsp; Then BITS_PER_WORD would be 32 and the array would need&nbsp; = 3 integer elements to hold 84 bits, and the “last” 12 bits in the third block would be unused.&nbsp; For simplicity in accessing bits, we will have bit 0 of the <strong>BitArray</strong> be bit 0 in the 0<sup>th</sup> integer block in the array, as the following diagram of bit positions illustrates:

<table width="701">
<tbody>
<tr>
<td width="234">31 30…

… 1 0
</td>
<td width="233">63 62…

… 33 32
</td>
<td width="234">&nbsp;(unused bits)&nbsp; 83 82…

… 65 64
</td>
</tr>
</tbody>
</table>
Although this layout does not reflect the logical order users visualize for a bit string, it makes easy work for you of setting and resetting bits by bitwise operations. Suppose, for example, a user has a <strong>BitArray</strong> object, <strong>b</strong>, and wants to <em>set</em> (i.e., turn “on”) the bit in position 50:

To implement this, your <strong>operator[ ]</strong> needs to determine that this bit position resides in array element 1 (the second “block”), and is bit number 18 offset from the right in that block. This, of course, is very easy:

You can then define the appropriate mask and change the second block (<strong>words[1]</strong>) in your array.

Naturally, users expect the bits to be processed <em>as if</em> they were stored positionally in increasing index order, <em>left-to-right</em> (so bit-0 is logically <em>left-most</em>), so any I/O functions (like <strong>operator&lt;&lt; </strong>and<strong> operator &gt;&gt;</strong>) should process them in that string-like order.

See the driver <a href="https://uvu.instructure.com/courses/489107/files/94257649/download"><strong><em>main.cpp</em></strong></a> <a href="https://uvu.instructure.com/courses/489107/files/94257649/download"><strong>(</strong></a><a href="https://uvu.instructure.com/courses/489107/files/94257649/download"><strong>https://uvu.instructure.com/courses/489107/files/94257649/download) </strong></a><a href="https://uvu.instructure.com/courses/489107/files/94257649/download">f</a>or examples.

<h1>Class Definition</h1>
The class interface you need to implement follows.

Remember that all of your code should reside in a header file (<em>bitarray.h</em>; that’s how templates work).&nbsp; If you refer to the <strong>BitArray</strong> <em>type </em>outside of the class definition, or if you create a local <strong>BitArray</strong> object, you must qualify it as <strong>BitArray</strong>&lt;<strong>IType</strong>&gt;.

Note that all single-argument constructors (except the copy constructor) are <strong>explicit</strong>, so all operator functions can be members (except the stream operators, of course).&nbsp; Define the bodies of the stream operators as friends inside the class definition itself (this is important for templates!).

The first constructor initializes a <strong>BitArray</strong> object to the appropriate number of 0-bits if its argument is greater than zero.&nbsp; The second constructor expects a string consisting only of characters ‘0’ and ‘1’ and builds the corresponding <strong>BitArray</strong> object with the bits set in the same logical configuration.

<h1>Stream Operators</h1>
Remember that if a stream contains <strong>0100abc</strong>, then the stream input operator (&gt;&gt;) will overwrite its <strong>BitArray</strong> argument with <strong>0100</strong> and leave <strong>abs</strong> in the stream, just like reading numbers does.&nbsp; Throw a <strong>runtime_error</strong> (declared in <strong>&lt;stdexcept&gt;)</strong> if any other characters occur in the input argument string (even whitespace).&nbsp; An empty string is okay, though (just create an empty object).&nbsp; For the input operator, set the stream to a fail state if there are no valid bit characters to be read in the input stream (after skipping white space, of course).

<h1>Bracket Operators/BitProxy</h1>
Throw a <strong>logic_error</strong> (also declared in <strong>&lt;stdexcept&gt;</strong>) if any out-of-range indexing is attempted anywhere.

Define a nested, private <strong>bitproxy</strong> class to accommodate intelligent use of <strong>operator[ ]</strong>, as discussed in class (i.e., distinguish between <strong>b[i]</strong>

<strong>= true</strong> and <strong>bool val = b[i]</strong>).&nbsp;&nbsp; See <a href="https://uvu.instructure.com/courses/489107/files/96193754/download"><strong><em>bits.cpp</em></strong></a> <a href="https://uvu.instructure.com/courses/489107/files/96193754/download"><strong>(</strong></a><a href="https://uvu.instructure.com/courses/489107/files/96193754/download"><strong>https://uvu.instructure.com/courses/489107/files/96193754/download) </strong></a><a href="https://uvu.instructure.com/courses/489107/files/96193754/download">i</a>n the code set for hints on how to define it.

&nbsp;

<h1>Other Program Notes</h1>
Move Construction/Assignment – You have two options with regards to how you leave the state of the ‘moved’ object:

<ol>
<li>Leave the ‘temp’ (moved) object in an initial state, eg., size() ==0, cleared vector etc.</li>
<li>Swap the internal contents completely between the two objects.</li>
</ol>
The <strong>shrink_to_fit</strong> function eliminates any unused blocks at the end of your storage vector that may have accrued after calls to <strong>erase</strong> (so you are, in effect, supporting an on-demand, “shrink-to-fit” storage allocation policy, but not forcing it).&nbsp; Just call vector::resize appropriately.

The comparison operators should compare <strong>BitArray</strong> objects <em>lexicographically</em> (i.e., as if they were strings, in dictionary order). The rest of the member functions should be self-explanatory.

Don’t convert your BitArray to a string using to_string() to implement comparisons or other operators such as insert, erase etc.&nbsp; It is possible, but defeats much of the purpose of the exercise.

<em>Professional tip</em>:&nbsp;&nbsp; Begin by implementing some private, low-level functions to handle individual bits in any position.&nbsp;&nbsp; See Program 6 <a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats">section of </a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>Pro</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>ram Hints and Caveats pa</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>e</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong> (https://uvu.instructure.com/courses/489107/pa</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>es/pro</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>ram-hints-and-</strong></a>

<a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>caveatshttps://uvu.instructure.com/courses/489107/pa</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>es/pro</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats"><strong>ram-hints-and-caveats) </strong></a><a href="https://uvu.instructure.com/courses/489107/pages/program-hints-and-caveatshttps:/uvu.instructure.com/courses/489107/pages/program-hints-and-caveats">for a list of these functions.&nbsp;&nbsp; Th</a>ey can then be used to great advantage in writing other functions.

&nbsp;

<h1>Testing and Submission</h1>
<a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206">There is a file, </a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><em>test.h</em></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206">, and a test program, main.cpp that you can download from Zylabs (or </a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>files-&gt;Pro</strong></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>ram 6</strong></a>

<a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>(https://uvu.instructure.com/courses/489107/files/folder/Pro</strong></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>rams/Pro</strong></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206"><strong>ram%206#) </strong></a><a href="https://uvu.instructure.com/courses/489107/files/folder/Programs/Program%206">).&nbsp;&nbsp; Use these to test your cod</a>e before you turn submit to Zylabs.&nbsp; The zylabs tests are based on the unit tests in main.cpp.&nbsp;&nbsp; It is far easier to run and test locally before submitting to Zylabs.&nbsp; The main.cpp output should look like:

move constructor move assignment move assignment move assignment move assignment move assignment move assignment shrinking from 2 to 1 words Test Report:

Number of Passes = 69

Number of Failures = 0

&nbsp;

Note the trace statements above the report.&nbsp; You should output ‘move assignment’, ‘move constructor’ in the move functions.&nbsp;&nbsp; shrink_to_fit should output as above also.

&nbsp;

FYI, my <em>bitarray.h</em> is about 350 lines of executable code.

&nbsp;

<h1>Grading/Rubric</h1>
<a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs">See our general </a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>Gradin</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong> Criteria for CS 3370 Pro</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>rams</strong></a> <a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>(</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>https://uvu.instructure.com/courses/489107/pa</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>es/</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>radin</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>-criteria-for-cs-</strong></a>

<a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>3370-pro</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>g</strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs"><strong>rams) </strong></a><a href="https://uvu.instructure.com/courses/489107/pages/grading-criteria-for-cs-3370-programs">&nbsp;for general deductions</a>

Program 6 will be submitted in Zylabs

Points awarded(100 pts total)

18 Unit Tests totaling 100 points

Deductions

Should not have explicit dependencies on type of integer used for the backing vector (e.g., 1u) -3

Ineffective us of std::vector methods to manage the size of the underlying vector of integers (especially resize)&nbsp;&nbsp; -2

Effective implementation of overloaded operators did not write some operators in terms of other operators;&nbsp; -2

&lt;&lt; should be written in terms of &lt;&lt;=, not visa versa -2 did not have low-level, private member functions for locating, reading, and writing individual bits);&nbsp; -3

A lot of extra move assignments from &lt;&lt;=, &gt;&gt;=, insert ops. should not use move assignment, just act on bitarray itself, e.g., resize, then read/assign. -4

excessive use of strings and temp objects for internal operations -3

Extra Credit is applied from second examplary requirement onwards.

Example,&nbsp; zylabs score 92, 1st exemplary req (+0), 2nd exemplary req (+2) = 94 Max score is capped at 100%

Exemplary Items

Simplest possible logic; utility functions like read_bit and assign_bit (and others) are used.&nbsp;&nbsp; +2

Correct implementation of move semantics;+2

Move Constructor leave internal contents of moved items in safe state (either swapped with left hand side, or zeroed out)

Efficient implementation of bitproxy class and the associated BitArray index operators +2

<h2>Assessment Rubric</h2>
<strong>Competency ↓&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Emerging →&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Proficient →&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Exemplary</strong>

Effective use of

<strong>std::vector</strong> methods to

manage the size of the

<em>Memory Management&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>

underlying vector of

integers (especially

<strong>resize</strong>)

Simplest possible logic to

No magic numbers (use&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; fulfill program

No repeated code

named constants and&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; requirements; utility

<em>Clean Code&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>(refactor); No

inline functions for&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; functions like <strong>read_bit</strong>

unnecessary code

program parameters)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; and <strong>assign_bit</strong> (and

others) are used.

Use <strong>assert</strong> in

<em>Defensive&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>Exceptions thrown as&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; appropriate places (I only

&nbsp;

<em>Programming&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>requested&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; have one, actually, in

<strong>read_bit</strong>)

Use a single type&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; No explicit dependencies

<em>Templates&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>parameter for the&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; on type of integer used

underlying integer type&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; for the backing vector

&nbsp;

Effective implementation of overloaded operators (beware repeated code; write some operators in terms of other operators; have low-level, private

<em>Other&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>

member functions for locating, reading, and writing individual bits); set stream state appropriately in operator&gt;&gt;

&nbsp;

Correct implementation of move semantics; efficient implementation of bitproxy class and the associated BitArray index operators
