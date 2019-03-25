## Behind the Scenes
<!-- .element: class="white-bg" -->


![Server](images/CE_server_2.jpg)<!-- .element: height="500" -->


<div>

## But really...

* Amazon Web Services
* 3-5 EC2 instances
* CloudFront
* Application Load Balancers
* EFS

</div><!-- .element: class="white-bg" -->


![Diag](images/ce_aws.svg)<!-- .element: class="no-border" -->


## CE stats
<!-- .element: class="white-bg" -->

![Stats](images/all_compilations_stats.png)<!-- .element: class="no-border stretch white-bg" -->


<div>

## CE stats

* 950k compilers per day
* 1.5/sec average
* 4/sec peak
* 3000 short URLs/day

</div><!-- .element: class="white-bg" -->


<div>

## Compiler stats

* 400+ compilers
* 250+GB

<div class="lang-container">
<div>Ada</div>
<div>Analysis</div>
<div>Assembly</div>
<div>C</div>
<div>C++</div>
<div>Clean</div>
<div>Cppx</div>
<div>CUDA</div>
<div>D</div>
<div>Fortran</div>
<div>Go</div>
<div>Haskell</div>
<div>ispc</div>
<div>LLVM IR</div>
<div>OCaml</div>
<div>Pascal</div>
<div>Rust</div>
<div>Swift</div>
<div>Zig</div>
</div><!-- -->

</div><!-- .element: class="white-bg" -->


## Maintaining

```bash
laptop$ ce admin

ubuntu@admin-node ~> ce --env prod instances list 

Address          State      Type       ELB     Service  Version       
34.226.244.207   running    t3.medium  healthy running  3965 (master) 
3.91.14.221      running    c5.large   healthy running  3965 (master) 
ubuntu@admin-node ~> ce --env prod builds list
Live  Branch     Version    Size       Hash          
 -->  master     3965       58.2MiB    969925..8b69c5
      master     3979       58.2MiB    9410c2..fbc044
      policy-... 3983       58.2MiB    27eccb..62da61

ubuntu@admin-node ~> ce --env prod builds set_current 3979
ubuntu@admin-node ~> ce --env prod instances restart
```


## Compilers

* Built with custom docker containers
* Daily process