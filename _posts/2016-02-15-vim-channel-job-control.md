---
layout: post
title:  "Vimのchannelとjob-control"
---
なんだかいい感じに動く様になってきた。今の所 Windows でもこんなのが動く様になってます。

```vim
let job = job_start("tee")
let handle = job_getchannel(job)
echo ch_sendraw(handle, "echo something\n")
call job_stop(job)
```

