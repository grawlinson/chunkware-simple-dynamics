cmake_minimum_required(VERSION 3.22)

project(ChunkwareSimpleDynamics VERSION 1.12 LANGUAGES CXX)

add_library(${PROJECT_NAME} STATIC)

target_sources(${PROJECT_NAME} PRIVATE
    simpleSource/SimpleComp.cpp
    simpleSource/SimpleComp.h
    simpleSource/SimpleCompProcess.inl
    simpleSource/SimpleEnvelope.cpp
    simpleSource/SimpleEnvelope.h
    simpleSource/SimpleGain.h
    simpleSource/SimpleGate.cpp
    simpleSource/SimpleGate.h
    simpleSource/SimpleGateProcess.inl
    simpleSource/SimpleHeader.h
    simpleSource/SimpleLimit.cpp
    simpleSource/SimpleLimit.h
    simpleSource/SimpleLimitProcess.inl
)

target_include_directories(${PROJECT_NAME} PUBLIC simpleSource)
