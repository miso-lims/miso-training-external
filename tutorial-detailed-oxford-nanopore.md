---
layout: page
category: walkthrough
title: Oxford Nanopore tutorial
is-detailed: true

---

<object data="presentations/miso_ont_training.pdf" width="800" height="500" type='application/pdf'> </object>


<div id="toc">
Table of Contents
<ol>
   <li><a href="#logging_in">Logging In</a></li>
   <li><a href="#project">Creating a Project</a></li>
   <li><a href="#libraries-receipt">Receiving Libraries</a></li>
   <li><a href="#pools">Pooling</a></li>
   <li><a href="#runs-new">Creating Runs</a></li>
</ol>
</div>

{% include logging_in.md detailed=page.is-detailed %}

<a name="scan" href="#" id="toplink">top</a>

{% include ont_project.md detailed=page.is-detailed %}

{% include libraries-receipt.md detailed=page.is-detailed section=3 platform='Oxford Nanopore'
  type=site.ont_library_type %}

{% include ont_pools.md detailed=page.is-detailed %}

{% include runs-new.md section=5 flowcell=site.ont_flowcell sequencer=site.ont_sequencer
  platform=site.ont_platform platform_type='Oxford Nanopore' seq_params=site.ont_seq_params %}

{% include ont_runs_add_pools.md %}

< <a href="tutorial-detailed-arrays">Arrays</a> | <a href="index">Home</a>
