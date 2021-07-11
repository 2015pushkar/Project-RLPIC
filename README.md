<p>#t_var = number of different values of t</p>
<p> #n_var = number of different values of number of clients</p>
 mat[][] of dim(t_var,n_var) 
 for t in range 1:9:2:
 for n in range 25:1000:25:
 numOfphases = []*200
 for iter over 200 iterations:
 ~ Phase_count = 0
 ~ fix the number of packets
 ~ fix the packet length
 ~ Generate Random Packets 
 ~ Generate Random Side Info Matrix
 ~ Based on Matrix,Update clients` packets
 ~ Convert bits to BPSK scheme
 ~ Call Pliable Demand Satisfaction Check block
 ~ Until it returns true:
 - Access 2 clients at a time:
 ~ Call Packets Selection Block.
 ~ Phase_count += 1
 ~ for each bit in packet:
 - Execute Part 1 Block
 - Execute Part 2 Phase Block.
 - Update Clients` packet.
 ~ Update the Side Info Matrix
 ~ numOfphases[iter] = Phase_count
 - Avg = avg(numOfphases)
 - mat[t][n] = Avg
