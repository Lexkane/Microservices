# microservice message processor in rust
Example project rust microservice for storing user messages

How to build

1.Download rustlang via curl https://sh.rustup.rs -sSf | sh

2.Switch to nightly version via rustup default nightly

3.Run update with rustup update

4.Set DEFAULT_DATABASE_PASSWORD to your postgres password
you can connect to diffrent database if you edit the connection string

5.Create Database messages from schemas folder

6.Run cargo build --release

7.If u want u can reduce binary size even more

You can use dynamic linking with: cargo rustc --release -- -C prefer-dynamic

This will dramatically reduce the size of the binary, as it is now dynamically linked. On Linux, you can also strip the binary of symbols using the strip command: strip target/release/microservice_rs

8.Enjoy your rust binary got extra small from  5mb to  2mb. 

This what you can call a <<real>> microservice
