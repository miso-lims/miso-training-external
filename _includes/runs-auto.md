<a name="runs-auto" href="#" id="toplink">top</a>

# 5. Working with automatically created runs

This exercise looks at a run created by Run Scanner. If your site is not using Run Scanner, you should skip this
exercise.

Shortly after an instrument begins imaging, MISO should detect it
and create a _Run_. As sequencing continues, MISO will pull back information
about the quality of the run similar to the on-instrument applications like SAV.
This includes statistics like percent pass filter, the percent of bases with
Qscores over 30, and cluster density.

1. From the _Sequencing Runs_ page, find the run `{{ site.run_scanner_run }}`.
   Click on the run alias to go to the run page.
1. Scroll down to the _Metrics_ section and examine the sequencing metrics for
   this run.

<a href="pics/metrics.png"><img style="width:100%;" src="pics/metrics.png"/></a>
