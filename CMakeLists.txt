cmake_minimum_required(VERSION 3.10)
project(ATMInterface)


set(CMAKE_CXX_STANDARD 17)

# Add the library
add_library(ATMInterface
    source/ATM.cpp
    source/CardReader.cpp
    source/CashDispenser.cpp
    source/ReceiptPrinter.cpp
    source/BankDB.cpp
    source/Vault.cpp
    source/ATMScreen.cpp
    source/SoundUnit.cpp
    source/Logger.cpp
    source/TechnicalSupport.cpp
    source/WithdrawTransaction.cpp
    source/DepositTransaction.cpp
    source/ATMConstants.cpp
)

# Include directories
target_include_directories(ATMInterface PUBLIC include/)



# export it as a library for another usage