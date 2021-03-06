set(LLVM_TARGET_DEFINITIONS CallInterfaces.td)
mlir_tablegen(CallInterfaces.h.inc -gen-op-interface-decls)
mlir_tablegen(CallInterfaces.cpp.inc -gen-op-interface-defs)
add_public_tablegen_target(MLIRCallInterfacesIncGen)

set(LLVM_TARGET_DEFINITIONS ControlFlowInterfaces.td)
mlir_tablegen(ControlFlowInterfaces.h.inc -gen-op-interface-decls)
mlir_tablegen(ControlFlowInterfaces.cpp.inc -gen-op-interface-defs)
add_public_tablegen_target(MLIRControlFlowInterfacesIncGen)

set(LLVM_TARGET_DEFINITIONS DerivedAttributeOpInterface.td)
mlir_tablegen(DerivedAttributeOpInterface.h.inc -gen-op-interface-decls)
mlir_tablegen(DerivedAttributeOpInterface.cpp.inc -gen-op-interface-defs)
add_public_tablegen_target(MLIRDerivedAttributeOpInterfaceIncGen)

set(LLVM_TARGET_DEFINITIONS InferTypeOpInterface.td)
mlir_tablegen(InferTypeOpInterface.h.inc -gen-op-interface-decls)
mlir_tablegen(InferTypeOpInterface.cpp.inc -gen-op-interface-defs)
add_public_tablegen_target(MLIRInferTypeOpInterfaceIncGen)

set(LLVM_TARGET_DEFINITIONS LoopLikeInterface.td)
mlir_tablegen(LoopLikeInterface.h.inc -gen-op-interface-decls)
mlir_tablegen(LoopLikeInterface.cpp.inc -gen-op-interface-defs)
add_public_tablegen_target(MLIRLoopLikeInterfaceIncGen)

set(LLVM_TARGET_DEFINITIONS SideEffects.td)
mlir_tablegen(SideEffectInterfaces.h.inc -gen-op-interface-decls)
mlir_tablegen(SideEffectInterfaces.cpp.inc -gen-op-interface-defs)
add_public_tablegen_target(MLIRSideEffectOpInterfacesIncGen)

set(LLVM_TARGET_DEFINITIONS ViewLikeInterface.td)
mlir_tablegen(ViewLikeInterface.h.inc -gen-op-interface-decls)
mlir_tablegen(ViewLikeInterface.cpp.inc -gen-op-interface-defs)
add_public_tablegen_target(MLIRViewLikeInterfaceIncGen)
