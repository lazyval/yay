Over the past several years of working with hadoop CLI tools I got totally tired of awful UX I had. Just to mention a few quirks: 
 - slow startup times: every command incurs a JVM startup so more often than not actual execution timings are higher than the time it takes to spin up new VM
 - lack of auto-complete for many of the scenarious (what a drag!)
 - suboptimal implementation of some of the commands (`hdfs dfs -ls` is able to OOM even though it's not supposed to -- it's work is purely iterative and not supposed to suck in everything it code in memory)
 - non-friendliness to automation (e.g. output format friendly to parsing)

So I am desperate to find how much effort it will take to tackle this and other deep-rooted issues of hadoop ecosystem CLI tools and this project is an attempt to find this out. 
