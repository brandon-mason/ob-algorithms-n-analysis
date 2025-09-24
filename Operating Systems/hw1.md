# 5
a) 
- Command: top
- Utilization: 1069.9MiB / 15733.2MiB

b) 
- Command: pstree 810066 -s -p
- Output: systemd(1)───sshd(789024)───sshd(809613)───sshd(809650)───bash(809651)───pstree(810066)

c) 
- Command: ps -U root | wc -l
- Output: 163

d) top