Download Link: https://assignmentchef.com/product/solved-howler
<br>
<a href="https://www.youtube.com/playlist?list=PLhOuww6rJJNNzo5zqtx0388myQkUKyrQz" rel="nofollow">https://www.youtube.com/playlist?list=PLhOuww6rJJNNzo5zqtx0388myQkUKyrQz</a>

Write a program that uppercases the given text:

<pre><code>$ ./howler.py 'The quick brown fox jumps over the lazy dog.'THE QUICK BROWN FOX JUMPS OVER THE LAZY DOG.</code></pre>

If the text names a file, uppercase the contents of the file:

<pre><code>$ ./howler.py ../inputs/fox.txtTHE QUICK BROWN FOX JUMPS OVER THE LAZY DOG.</code></pre>

If given no arguments, print a brief usage:

<pre><code>$ ./howler.pyusage: howler.py [-h] [-o str] strhowler.py: error: the following arguments are required: str</code></pre>

If the <code>-o</code> or <code>--outfile</code> option is present, write the output to the given file and print nothing:

<pre><code>$ ./howler.py ../inputs/fox.txt -o out.txt</code></pre>

There should now be an <code>out.txt</code> file with the contents:

<pre><code>$ cat out.txtTHE QUICK BROWN FOX JUMPS OVER THE LAZY DOG.</code></pre>

Respond to <code>-h</code> or <code>--help</code> with a longer usage:

<pre><code>$ ./howler.py -husage: howler.py [-h] [-o str] strHowler (upper-cases input)positional arguments:  str                   Input string or fileoptional arguments:  -h, --help            show this help message and exit  -o str, --outfile str                        Output filename (default: )</code></pre>

Run the test suite to ensure your program is working correctly:

<pre><code>$ make testpytest -xv test.py============================= test session starts ==============================...collected 5 itemstest.py::test_exists PASSED                                              [ 20%]test.py::test_usage PASSED                                               [ 40%]test.py::test_text_stdout PASSED                                         [ 60%]test.py::test_text_outfile PASSED                                        [ 80%]test.py::test_file PASSED                                                [100%]============================== 5 passed in 0.40s ===============================</code></pre>