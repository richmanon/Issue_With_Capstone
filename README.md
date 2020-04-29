### Issue_With_Capstone
<pre>Capstone is a free, multiplatform and multi-architecture disassembler engine Disassemblers try to create the
assembly code from the binary machine code.</br>
We are using Operating sytem linux,python for front end ,C++ for backend ,capstone is a dissasembler thats the reason why we were using the 
capstone for lifitng the cfg file and our lfting process is written in C++ language.</pre>

### Reason why we are not able to implement the capstone

<B># Not Having Suitable API In C++ Language</B></BR>
<PRE>
    We are using C++ for lifting but capstone does not have suitable C++ api for the linux host but it has c++ wrapper for window. 
    But our OS is linux thats the reason we cant use capstone.Even if want to use cpastone for C++ for host OS linux then we have to implement
    C++ wrapper classs which is time consuming</PRE>
<VB># Cant Read CFG File</B></br>
<pre>
  We can only give raw binary bits to the capstone as an input.We cannot give cfg file as an input to capstone.Our tool front-end is producing a 
  CFG file which is to be given to capstone to disassemble  but capstone does not take CFG as input.</pre>
  </pre>
  
  ### References
  <pre>
  https://sourceforge.net/p/capstone/mailman/message/34538072/</br>
  https://github.com/aquynh/capstone</br>
  https://github.com/aquynh/capstone/tree/master/docs</pre>
