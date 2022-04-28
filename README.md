# protobuf_encode_decode_example
protobuf_encode_decode_example

1. encode to string or array 
2. send over protocol
3. receive and decode 

In stall protobuf:
1. Download/Unzip protobuf.zip
2. ./configure && autogen.sh
3. make && sudo make install
Use: 
protoc -I=./ --cpp_out=./output ./addressbook.proto
g++ -c addressbook.pb.cc 
g++ -o test test.cpp addressbook.pb.o -lprotobuf
