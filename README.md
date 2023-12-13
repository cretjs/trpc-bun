# [tRPC](https://trpc.io/) + [Bun](https://bun.sh/)

```sh
git clone https://github.com/sachinraja/trpc-bun
cd trpc-bun
bun install
bun dx
```

The `bun dx` command will start the development server and open the app in your browser. Changes to the router are automatically reloaded using [`bun-livereload`](https://github.com/Jarred-Sumner/bun-livereload).

# bun1.0.16-trpc
autocannon -c 1000 -d 20 -p 100 http://localhost:5000/hello
Running 20s test @ http://localhost:5000/hello
1000 connections with 100 pipelining factor


┌─────────┬────────┬────────┬────────┬────────┬──────────┬───────────┬─────────┐
│ Stat    │ 2.5%   │ 50%    │ 97.5%  │ 99%    │ Avg      │ Stdev     │ Max     │
├─────────┼────────┼────────┼────────┼────────┼──────────┼───────────┼─────────┤
│ Latency │ 461 ms │ 597 ms │ 607 ms │ 695 ms │ 593.7 ms │ 100.99 ms │ 1879 ms │
└─────────┴────────┴────────┴────────┴────────┴──────────┴───────────┴─────────┘
┌───────────┬─────────┬─────────┬─────────┬─────────┬───────────┬──────────┬─────────┐
│ Stat      │ 1%      │ 2.5%    │ 50%     │ 97.5%   │ Avg       │ Stdev    │ Min     │
├───────────┼─────────┼─────────┼─────────┼─────────┼───────────┼──────────┼─────────┤
│ Req/Sec   │ 156,415 │ 156,415 │ 167,167 │ 168,319 │ 166,297.6 │ 2,731.87 │ 156,298 │
├───────────┼─────────┼─────────┼─────────┼─────────┼───────────┼──────────┼─────────┤
│ Bytes/Sec │ 26.1 MB │ 26.1 MB │ 27.9 MB │ 28.1 MB │ 27.8 MB   │ 456 kB   │ 26.1 MB │
└───────────┴─────────┴─────────┴─────────┴─────────┴───────────┴──────────┴─────────┘

Req/Bytes counts sampled once per second.
# of samples: 20

3426k requests in 20.14s, 555 MB read