add_library(Block BlockBase.cpp DSBlock.cpp MicroBlock.cpp TxBlock.cpp)
target_include_directories(Block PUBLIC ${PROJECT_SOURCE_DIR}/src)
target_link_libraries (Block LINK_PUBLIC Crypto Trie)