!!!
Attention this is an unsupported fork.
Original readme -> README.md.orig
!!!


Modified by Alexander Sherikov, 2014.10.20:
    - changed CMakeLists.txt -- now cmake expects the path to Eigen to be
      specified by the user.
    

Reason:
    The master branch of SOTH does not support Eigen >= 3.2, the branch that
    implements this support is stale.


clone & build:
    git clone https://github.com/asherikov/soth.git
    git submodule update --init --recursive
    mkdir _build
    cd _build
    cmake .. -DEIGEN_INCLUDE_DIR=<path_to_eigen>
    make
