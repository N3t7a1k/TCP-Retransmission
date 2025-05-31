# TCP Retransmission

## Idea

If client receive data from it's receive socket buffer before retransmission, client will take the original data.

But, if not it depends on how OS's kernel controls.

What happens if retransmitted data is different from original data?

![idea](https://n3t7a1k.io/posts/tcp-%EC%9E%AC%EC%A0%84%EC%86%A1-%EC%8B%A4%ED%97%98/media/tcp-retransmission.png)

## Result

As a result operating systems that I could test(Windows, Linux) didn't update payload to retransmitted data.

You can check out the packets I captured in testing [here](retransmit.pcapng).

