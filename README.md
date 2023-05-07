Download Link: https://assignmentchef.com/product/solved-me759-assignment-1
<br>
<ol>

 <li>(a) Read the files md and slurm usage.md from the general directory of the <a href="https://github.com/nicolsen/ME759-2020/">ME759 </a><a href="https://github.com/nicolsen/ME759-2020/">Resource Repo</a><a href="https://github.com/nicolsen/ME759-2020/">.</a> These are very important documents of the expectations for your assignments throughout the semester.

  <ul>

   <li>Read the hw repos.md file and follow the instructions to create an account. This is very important and must be done in order for you to have a way to turn in HW02.</li>

   <li>At least skim md. This contains a quick guide for effectively working between your local computer and Euler.</li>

  </ul></li>

 <li>Write a single line of bash for each of the following (you can use pipes and/or redirects). Pretend that any files or directories mentioned exist (don’t turn them in).

  <ol>

   <li>Print the current working directory</li>

   <li>Change directories into a directory called somedir</li>

   <li>List the names of all files in the current directory</li>

   <li>(Optional) Write a for loop which prints each integer 0 to 10.</li>

   <li>(Optional) Print the names of all files ending in .txt in the current directory or any of its subtree</li>

   <li>(Optional) Print the last 2 lines of a plain text file in the current directory called txt</li>

   <li>(Optional) Print the entire contents of a file in the current directory called txt</li>

  </ol></li>

 <li>Using Euler and the module command, answer the following questions.

  <ol>

   <li>Are there any modules loaded (module list) when you log in?</li>

   <li>What version (version number) of gcc is available to you without loading any modules?</li>

   <li>List all gcc modules available on Euler.</li>

   <li>Which gcc module is loaded when you run module load gcc and what version number of gcc is loaded by that module?</li>

   <li>List one other piece of software that you know that has a module on Euler and one sentence about what it does. (If you aren’t familiar with any of the other software, look one up and write a sentence about it.)</li>

  </ol></li>

 <li>Write a bash script called sh with a Slurm header which asks for

  <ul>

   <li>2 CPU cores</li>

   <li>A job name of FirstSlurm</li>

   <li>An output file called out</li>

   <li>An error file called err</li>

  </ul></li>

</ol>

and runs a single command to print the hostname of the machine (compute node) running the job. This job should be submittable by running sbatch task4.sh on the head node.

<ol start="5">

 <li>Research some useful Slurm tools (one sentence responses):

  <ol>

   <li>Explain what SLURM SUBMIT DIR is in the environment of a running Slurm job.</li>

   <li>In what directory does a Slurm job on euler begin execution. You should run some jobs to check this?</li>

   <li>Explain what SLURM JOB ID is in the environment of a running Slurm job.</li>

   <li>Explain what the following script header line specifies: #SBATCH –array=0-9</li>

   <li>Explain what SLURM ARRAY TASK ID is in the environment of a running Slurm job with</li>

  </ol></li>

</ol>

the header from part (d).

<ol>

 <li>Explain what the following script header line specifies: #SBATCH –gres=gpu:1</li>

</ol>

<ol start="6">

 <li>Write a C++ program called cpp which takes a command line argument N, and prints out each integer from 0 to N (including 0 and N) separated by spaces on a single line ending in a newline.

  <ul>

   <li>Compile command: g++ task6.cpp -Wall -O3 -o task6</li>

   <li>Run command: ./task6 N</li>

   <li>Expected output (followed by newline): 0 1 2 3 ·· N</li>

   <li>Expected output for N = 6 (followed by newline): 0 1 2 3 4 5 6</li>

  </ul></li>

</ol>