#Constant op 생성하기
hello = tf.constant('Hello, TensorFlow!')

#TF session 생성하기
sess = tf.Session()

#run the op and get result // 'print' is for getting result 
print(sess.run(hello))

##---Create Computational Graph---##
node1 = tf.constant(3.0, tf.float32)
node2 = tf.constant(4.0) #also tf.float32 implicitly
node3 = tf.add(node1, node2) #node1과 node2 합침

print("NODE1:", node1, "NODE2:", node2)
print("NODE3:", node3)

sess = tf.Session()
print("sess.run(node1, node2): ", sess.run([node1, node2]))
print("sess.run(node3): ", sess.fun(node3))
