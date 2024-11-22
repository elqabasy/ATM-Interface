cmake_minimum_required(VERSION 3.10)
project(ATMInterface)


set(CMAKE_CXX_STANDARD 17)

# Add the library
add_library(ATMInterface
    src/ATM.cpp
    src/CardReader.cpp
    src/CashDispenser.cpp
    src/ReceiptPrinter.cpp
    src/BankDB.cpp
    src/Vault.cpp
    src/ATMScreen.cpp
    src/SoundUnit.cpp
    src/Logger.cpp
    src/TechnicalSupport.cpp
    src/WithdrawTransaction.cpp
    src/DepositTransaction.cpp
    src/ATMConstants.cpp
)

# Include directories
target_include_directories(ATMInterface PUBLIC include/)



# export it as a library for another usage