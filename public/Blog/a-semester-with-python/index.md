# A Semester with Python



<div id="TOC">
no
</div>

<!--more-->
<p>Here are some example of what I did with Python during my time in SDS348.</p>
<p>Python is one of the most popular languages used in the computer science realm. Since it can get complex real quick, it is important to first get the hang of some of the more basic codes. Here are some basic codes to get you adjusted to Python</p>
<pre class="python"><code>print(&quot;hello world&quot;)</code></pre>
<pre><code>## hello world</code></pre>
<p>By importing numpy as np, we can even use python to perform basic calculations! Python can also be used to assign values to variables.This is why Python is so popular!!</p>
<pre class="python"><code>import numpy as np
2+2</code></pre>
<pre><code>## 4</code></pre>
<pre class="python"><code>4+4</code></pre>
<pre><code>## 8</code></pre>
<pre class="python"><code>three = 3
two = 2
two * three</code></pre>
<pre><code>## 6</code></pre>
<p>Here are some more Challenging python codes.</p>
<pre class="python"><code>my_seq1 = &quot;ATCATCATG&quot;
my_seq2 = &quot;CAGCCCAATCAGGCTCTACTGCCACTAAACTTACGCAGGATATATTTACGCCGACGTACT&quot;

def count_kmers(read, k):
    
 
    counts = {}
  
    num_kmers = len(read) - k + 1
   
    for i in range(num_kmers):
     
        kmer = read[i:i+k]
      
        if kmer not in counts:
            counts[kmer] = 0

        counts[kmer] += 1
 
    return counts

# my_seq1
count_kmers(&quot;ATCATCATG&quot;,3)</code></pre>
<pre><code>## {&#39;ATG&#39;: 1, &#39;CAT&#39;: 2, &#39;ATC&#39;: 2, &#39;TCA&#39;: 2}</code></pre>
<pre class="python"><code>def count_kmers(read, k):
    
 
    counts = {}
  
    num_kmers = len(read) - k + 1
   
    for i in range(num_kmers):
     
        kmer = read[i:i+k]
      
        if kmer not in counts:
            counts[kmer] = 0

        counts[kmer] += 1
 
    return counts

count_kmers(&quot;CAGCCCAATCAGGCTCTACTGCCACTAAACTTACGCAGGATATATTTACGCCGACGTACT&quot;,3)</code></pre>
<pre><code>## {&#39;CTT&#39;: 1, &#39;AAA&#39;: 1, &#39;ATC&#39;: 1, &#39;AAC&#39;: 1, &#39;ATA&#39;: 2, &#39;AGG&#39;: 2, &#39;CTC&#39;: 1, &#39;AGC&#39;: 1, &#39;AAT&#39;: 1, &#39;ATT&#39;: 1, &#39;CTG&#39;: 1, &#39;CTA&#39;: 2, &#39;ACT&#39;: 4, &#39;CAC&#39;: 1, &#39;ACG&#39;: 3, &#39;CAA&#39;: 1, &#39;CCA&#39;: 2, &#39;CCG&#39;: 1, &#39;CCC&#39;: 1, &#39;TAT&#39;: 2, &#39;CGA&#39;: 1, &#39;CAG&#39;: 3, &#39;TCT&#39;: 1, &#39;GAT&#39;: 1, &#39;TTT&#39;: 1, &#39;TGC&#39;: 1, &#39;GGA&#39;: 1, &#39;TAA&#39;: 1, &#39;GGC&#39;: 1, &#39;TAC&#39;: 4, &#39;TTA&#39;: 2, &#39;GAC&#39;: 1, &#39;CGT&#39;: 1, &#39;TCA&#39;: 1, &#39;GCA&#39;: 1, &#39;GTA&#39;: 1, &#39;GCC&#39;: 3, &#39;GCT&#39;: 1, &#39;CGC&#39;: 2}</code></pre>
<p>This code chunk was used to find k-mers of certain sequences. So as you can see, Python can be use in many different ways. This revolutionary coding language makes things easier for people new to coding and even experienced one as well.</p>
