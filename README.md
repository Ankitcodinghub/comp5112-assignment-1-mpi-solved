# comp5112-assignment-1-mpi-solved
**TO GET THIS SOLUTION VISIT:** [COMP5112 Assignment 1-MPI Solved](https://www.ankitcodinghub.com/product/comp5112-assignment-1-mpi-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91302&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;COMP5112 Assignment 1-MPI Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 0px;">
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
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="section">
<div class="layoutArea">
<div class="column">
&nbsp;

Assignment Description

Graph structural clustering is a common data analysis task to cluster vertices by their edge connections in the graph. SCAN (Structural Clustering Algorithm for Networks) [1] is such an algorithm that clusters vertices based on a structural similarity measure. The algorithm is efficient in both computation and memory.

In this assignment, you will implement an MPI program to perform clustering on multiple graphs by calling our provided sequential SCAN function in each MPI process.

In the SCAN implementation, each graph is stored in a CSR structure, illustrated as follows:

</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="section">
<div class="layoutArea">
<div class="column">
where one array is used to store the neighborhood information in sequential order, and the other array stores the offset for corresponding vertex.

Note: The length of array for storing offsets is the number of vertices plus one, as the first element of vertices is zero and points to the first element of the array of neighbors. Accordingly, the length of array for storing neighbors is the number of edges plus one.

The code skeleton clustering_mpi_skeleton.cpp is provided. Your task is to complete the missing code in the main function. Specifically, you need to:

<ol>
<li>Scatter the information of the graphs to each process.</li>
<li>Perform clustering in parallel.</li>
<li>Gather the results to the master process, which contain both number of clusters and cluster index of each vertex.</li>
<li>Output the clustering results to both screen and files (see the provided sequential version for details).
Package list
</li>
</ol>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>assignment1-package/
  ├── datasets
  |   ├── test1
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<ul>
<li>| &nbsp;|</li>
<li>| &nbsp;|</li>
<li>| &nbsp;|</li>
<li>| &nbsp;|</li>
<li>| &nbsp;├── test2</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>├── meta
├── 1.txt
├── ...
└── 12.txt
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<ul>
<li>| &nbsp;|</li>
<li>| &nbsp;|</li>
<li>| &nbsp;|</li>
<li>
<pre>| &nbsp;  |
├── results
├── clustering_h.cpp
├── clustering_mpi_skeleton.cpp
├── clustering_impl.cpp
</pre>
<pre>├── clustering_sequential.cpp
└── assignment1.pdf
</pre>
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>├── meta
├── 1.txt
├── ...
└── 12.txt
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<ol>
<li>datasets: sample input files of two test cases.

The input files of a test case are in the following format:

1. The number of graphs in the test case is stored in file meta.

2. Each graph is stored in a text file. The first line is “# nv ne”, where nv is the number of vertices and ne is the number

of edges of the graph, respectively. Each of the following lines is a pair of integers “v0 v1”, which represents an edge

(v0, v1) in the graph.
</li>
<li>clustering.h, clustering_impl.cpp: the source files of the SCAN implementation and some utilities.</li>
<li>clustering_sequential.cpp: the sequential implementation.</li>
<li>results: folder for saving the output results.</li>
</ol>
</div>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="section">
<div class="layoutArea">
<div class="column">
5. clustering_mpi_skeleton.cpp: MPI skeleton. 6. assignment1.pdf: the assignment description.

Note.1 The number of input graphs is assumed to be divisible by the number of processes. Each of the provided test cases contains 12 graphs.

Note.2 The clustering results of your MPI program should be the same as that of the provided sequential version.

Please complete the clustering_mpi_skeleton.cpp after the comment // ADD YOUR CODE HERE and make sure you only modify this file.

Please only submit clustering_mpi_skeleton.cpp to Canvas.

Compile and run

Sequential

&lt;test_folder&gt; is the path of the input files and &lt;result_folder&gt; is the path of the output results. E.g.,

MPI version

&lt;test_folder&gt; is the directory of the test files and &lt;result_folder&gt; is the path of the output results. &lt;num_process&gt; is the number of total processes. E.g.,

An example output is here for your reference:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>g++ clustering_sequential.cpp clustering_impl.cpp -o clustering_sequential -std=c++11 -g
-Wall
./clustering_sequential &lt;test_folder&gt; &lt;result_folder&gt;
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>./clustering_sequential ./dataset/test1/ ./results/
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>mpic++ -std=c++11 clustering_mpi_skeleton.cpp clustering_impl.cpp -o clustering
mpiexec -n &lt;num_processes&gt; ./clustering &lt;test_folder&gt;  &lt;result_folder&gt;
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>mpiexec -n 4 ./clustering ./dataset/test1 ./results/
</pre>
</div>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="section">
<div class="section">
<div class="layoutArea">
<div class="column">
And an example result file results/0.txt is output as follows:

where 3 is the number of total clusters and -1 0 1 2 is the cluster index for each vertex (-1 for not in any cluster).

Note: mpiexec may output warning about “unable to find network interfaces”. You can run the following command and re-

login the VM to suppress the warning.

References

1. Xu, Xiaowei, et al. “Scan: a structural clustering algorithm for networks.” Proceedings of the 13th ACM SIGKDD international conference on Knowledge discovery and data mining. 2007.

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>3
0 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 -1 2 2 2 2 2 2
</pre>
</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>echo "alias mpiexec='mpiexec -mca btl_base_warn_component_unused 0'" &gt;&gt; ~/.bashrc
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>num cluster in graph 0 : 3
num cluster in graph 1 : 2
num cluster in graph 2 : 3
num cluster in graph 3 : 2
num cluster in graph 4 : 2
num cluster in graph 5 : 2
num cluster in graph 6 : 3
num cluster in graph 7 : 3
num cluster in graph 8 : 2
num cluster in graph 9 : 3
num cluster in graph 10 : 3
num cluster in graph 11 : 3
Elapsed Time: 0.335364000 ms
</pre>
</div>
</div>
</div>
</div>
</div>
