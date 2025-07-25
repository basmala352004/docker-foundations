****lifecycle****

- docker create --name my-nginx nginx
- docker start my-nginx 
- docker system df 
TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          4         4         1.865GB   74.81MB (4%)
Containers      4         2         2.304MB   2.302MB (99%)
Local Volumes   7         2         1.473GB   439.1MB (29%)
Build Cache     8         0         342B      342B

- docker stop my-nginx
- docker rm my-nginx
- docker image prune -a
-  docker system df
TYPE            TOTAL     ACTIVE    SIZE      RECLAIMABLE
Images          3         3         1.747GB   0B (0%)
Containers      3         1         2.303MB   2.302MB (99%)
Local Volumes   7         2         1.473GB   439.1MB (29%)
Build Cache     8         0         342B      342B