# Comparing `tmp/quil-0.7.1rc0.tar.gz` & `tmp/quil-0.8.0.tar.gz`

## Comparing `quil-0.7.1rc0.tar` & `quil-0.8.0.tar`

### file list

```diff
@@ -1,208 +1,209 @@
--rw-r--r--   0     1001      127     1406 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/Cargo.toml
--rw-r--r--   0     1001      127    43450 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/CHANGELOG.md
--rw-r--r--   0     1001      127      954 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/README.md
--rw-r--r--   0     1001      127     1692 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/benches/corpus.rs
--rw-r--r--   0     1001      127      941 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/benches/get_frames_for_instruction.rs
--rw-r--r--   0     1001      127      985 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/benches/parser.rs
--rw-r--r--   0     1001      127   803952 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/benches/sample-calibrations.quil
--rw-r--r--   0     1001      127     1478 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/benches/scheduled_program_from_program.rs
--rw-r--r--   0     1001      127      969 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/benches/simplification.rs
--rw-r--r--   0     1001      127    12979 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/benches/test_expressions.txt
--rw-r--r--   0     1001      127     6316 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/examples/generate_test_expressions.rs
--rw-r--r--   0     1001      127    38082 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/expression/mod.rs
--rw-r--r--   0     1001      127    34338 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/expression/simplification/by_hand.rs
--rw-r--r--   0     1001      127    12745 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/expression/simplification/mod.rs
--rw-r--r--   0     1001      127     1002 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/hash.rs
--rw-r--r--   0     1001      127     4159 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     6478 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/circuit.rs
--rw-r--r--   0     1001      127     9937 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/classical.rs
--rw-r--r--   0     1001      127     5260 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     6939 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9857 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/frame.rs
--rw-r--r--   0     1001      127    43954 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/gate.rs
--rw-r--r--   0     1001      127      771 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/measurement.rs
--rw-r--r--   0     1001      127    39401 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1798 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/pragma.rs
--rw-r--r--   0     1001      127     3425 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      654 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/reset.rs
--rw-r--r--   0     1001      127      133 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
--rw-r--r--   0     1001      127      133 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
--rw-r--r--   0     1001      127      124 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
--rw-r--r--   0     1001      127      167 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
--rw-r--r--   0     1001      127      160 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
--rw-r--r--   0     1001      127      109 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
--rw-r--r--   0     1001      127      141 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
--rw-r--r--   0     1001      127      125 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
--rw-r--r--   0     1001      127      191 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
--rw-r--r--   0     1001      127      178 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
--rw-r--r--   0     1001      127      139 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
--rw-r--r--   0     1001      127      143 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
--rw-r--r--   0     1001      127     1528 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/timing.rs
--rw-r--r--   0     1001      127     3619 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1910 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/lib.rs
--rw-r--r--   0     1001      127     1013 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/macros.rs
--rw-r--r--   0     1001      127    36217 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/command.rs
--rw-r--r--   0     1001      127    23037 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/common.rs
--rw-r--r--   0     1001      127     5970 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/error/error.rs
--rw-r--r--   0     1001      127     2519 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/error/input.rs
--rw-r--r--   0     1001      127     3242 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/error/internal.rs
--rw-r--r--   0     1001      127     1004 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/error/kind.rs
--rw-r--r--   0     1001      127     2685 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/error/mod.rs
--rw-r--r--   0     1001      127    17487 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/expression.rs
--rw-r--r--   0     1001      127     2212 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/gate.rs
--rw-r--r--   0     1001      127    40956 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/instruction.rs
--rw-r--r--   0     1001      127     1380 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/lexer/error.rs
--rw-r--r--   0     1001      127    17439 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/lexer/mod.rs
--rw-r--r--   0     1001      127     4222 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/lexer/quoted_strings.rs
--rw-r--r--   0     1001      127     3357 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs
--rw-r--r--   0     1001      127     4162 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/macros.rs
--rw-r--r--   0     1001      127     2446 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/mod.rs
--rw-r--r--   0     1001      127     5841 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/parser/token.rs
--rw-r--r--   0     1001      127    25985 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/analysis/control_flow_graph.rs
--rw-r--r--   0     1001      127      974 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/analysis/mod.rs
--rw-r--r--   0     1001      127     9591 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/analysis/qubit_graph.rs
--rw-r--r--   0     1001      127      889 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
--rw-r--r--   0     1001      127     1329 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/analysis/test_programs.rs
--rw-r--r--   0     1001      127    22890 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/calibration.rs
--rw-r--r--   0     1001      127     2283 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/error/leftover.rs
--rw-r--r--   0     1001      127     3068 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/error/mod.rs
--rw-r--r--   0     1001      127     2252 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/error/result.rs
--rw-r--r--   0     1001      127     2725 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/error/syntax.rs
--rw-r--r--   0     1001      127     8742 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/frame.rs
--rw-r--r--   0     1001      127    17109 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/memory.rs
--rw-r--r--   0     1001      127    47063 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/mod.rs
--rw-r--r--   0     1001      127    26031 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/graph.rs
--rw-r--r--   0     1001      127    20046 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/graphviz_dot.rs
--rw-r--r--   0     1001      127      456 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/mod.rs
--rw-r--r--   0     1001      127    16670 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/schedule.rs
--rw-r--r--   0     1001      127     2678 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
--rw-r--r--   0     1001      127     1560 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
--rw-r--r--   0     1001      127     1166 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
--rw-r--r--   0     1001      127     1732 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
--rw-r--r--   0     1001      127     1112 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
--rw-r--r--   0     1001      127     1195 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
--rw-r--r--   0     1001      127     1780 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
--rw-r--r--   0     1001      127     1653 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
--rw-r--r--   0     1001      127     1003 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
--rw-r--r--   0     1001      127     1032 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
--rw-r--r--   0     1001      127      552 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
--rw-r--r--   0     1001      127     1540 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
--rw-r--r--   0     1001      127     1073 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
--rw-r--r--   0     1001      127     1338 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
--rw-r--r--   0     1001      127     1866 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
--rw-r--r--   0     1001      127      854 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
--rw-r--r--   0     1001      127      867 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
--rw-r--r--   0     1001      127      887 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
--rw-r--r--   0     1001      127     1892 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
--rw-r--r--   0     1001      127      839 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
--rw-r--r--   0     1001      127      768 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
--rw-r--r--   0     1001      127      591 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
--rw-r--r--   0     1001      127      793 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
--rw-r--r--   0     1001      127      852 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
--rw-r--r--   0     1001      127      585 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
--rw-r--r--   0     1001      127      227 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
--rw-r--r--   0     1001      127      136 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
--rw-r--r--   0     1001      127      215 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
--rw-r--r--   0     1001      127      476 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
--rw-r--r--   0     1001      127      210 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
--rw-r--r--   0     1001      127      141 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
--rw-r--r--   0     1001      127      159 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
--rw-r--r--   0     1001      127      353 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
--rw-r--r--   0     1001      127      302 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
--rw-r--r--   0     1001      127      199 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
--rw-r--r--   0     1001      127      254 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
--rw-r--r--   0     1001      127      174 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
--rw-r--r--   0     1001      127      167 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
--rw-r--r--   0     1001      127     3755 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
--rw-r--r--   0     1001      127      425 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
--rw-r--r--   0     1001      127    35007 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/program/type_check.rs
--rw-r--r--   0     1001      127     2422 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/quil.rs
--rw-r--r--   0     1001      127     2716 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/reserved.rs
--rw-r--r--   0     1001      127     2109 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/validation/identifier.rs
--rw-r--r--   0     1001      127       20 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/src/validation/mod.rs
--rw-r--r--   0     1001      127      724 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/calibration_test.rs
--rw-r--r--   0     1001      127      742 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/programs/calibration_cz.quil
--rw-r--r--   0     1001      127     1888 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/programs/calibration_cz_phase.quil
--rw-r--r--   0     1001      127     3266 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/programs/calibration_measure.quil
--rw-r--r--   0     1001      127     1588 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/programs/calibration_rx.quil
--rw-r--r--   0     1001      127     1786 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/programs/calibration_xy.quil
--rw-r--r--   0     1001      127      747 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
--rw-r--r--   0     1001      127     1797 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
--rw-r--r--   0     1001      127     3187 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
--rw-r--r--   0     1001      127     1519 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
--rw-r--r--   0     1001      127     1719 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 quil-0.7.1rc0/quil-py/Cargo.toml
--rw-r--r--   0     1001      127      203 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/.flake8
--rw-r--r--   0     1001      127       10 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/.stubtest-allowlist
--rw-r--r--   0     1001      127    19844 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/CHANGELOG.md
--rw-r--r--   0     1001      127      858 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/Makefile.toml
--rw-r--r--   0     1001      127      777 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/README-py.md
--rw-r--r--   0     1001      127      337 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/README.md
--rw-r--r--   0     1001      127       71 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/build.rs
--rw-r--r--   0     1001      127      404 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/make_docs.py
--rw-r--r--   0     1001      127      135 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/out/index.html
--rw-r--r--   0     1001      127    34673 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/out/quil/quil.html
--rw-r--r--   0     1001      127    34581 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/out/quil.html
--rw-r--r--   0     1001      127    20706 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/out/search.js
--rw-r--r--   0     1001      127    36038 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/poetry.lock
--rw-r--r--   0     1001      127      283 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/__init__.pyi
--rw-r--r--   0     1001      127       30 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7690 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127      124 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91321 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127      129 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/program/__init__.py
--rw-r--r--   0     1001      127    17921 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/program/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/py.typed
--rw-r--r--   0     1001      127      161 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/validation/__init__.py
--rw-r--r--   0     1001      127       39 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127       41 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/validation/identifier.py
--rw-r--r--   0     1001      127      439 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127    34593 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/quil.html
--rw-r--r--   0     1001      127     6656 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/expression.rs
--rw-r--r--   0     1001      127     2838 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/calibration.rs
--rw-r--r--   0     1001      127     1251 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/circuit.rs
--rw-r--r--   0     1001      127    11440 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/classical.rs
--rw-r--r--   0     1001      127     4295 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/control_flow.rs
--rw-r--r--   0     1001      127     5561 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/declaration.rs
--rw-r--r--   0     1001      127     9528 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/frame.rs
--rw-r--r--   0     1001      127     8394 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/gate.rs
--rw-r--r--   0     1001      127     1056 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/measurement.rs
--rw-r--r--   0     1001      127     8741 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/mod.rs
--rw-r--r--   0     1001      127     1852 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/pragma.rs
--rw-r--r--   0     1001      127      978 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/qubit.rs
--rw-r--r--   0     1001      127      738 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/reset.rs
--rw-r--r--   0     1001      127     1591 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/timing.rs
--rw-r--r--   0     1001      127     2434 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/instruction/waveform.rs
--rw-r--r--   0     1001      127     1967 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/lib.rs
--rw-r--r--   0     1001      127     2701 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/program/analysis.rs
--rw-r--r--   0     1001      127     3721 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/program/calibration.rs
--rw-r--r--   0     1001      127     2774 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/program/frame.rs
--rw-r--r--   0     1001      127      897 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/program/memory.rs
--rw-r--r--   0     1001      127    12666 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/program/mod.rs
--rw-r--r--   0     1001      127     1696 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/program/scheduling.rs
--rw-r--r--   0     1001      127     1136 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/validation/identifier.rs
--rw-r--r--   0     1001      127      151 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/src/validation/mod.rs
--rw-r--r--   0     1001      127     1665 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/test/instructions/test_copy.py
--rw-r--r--   0     1001      127      351 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/test/instructions/test_gate.py
--rw-r--r--   0     1001      127      137 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/test/program/__snapshots__/test_program.ambr
--rw-r--r--   0     1001      127     4566 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/test/program/test_program.py
--rw-r--r--   0     1001      127     1023 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil-py/test/test_eq.py
--rw-r--r--   0     1001      127    47419 2024-03-19 00:35:15.000000 quil-0.7.1rc0/Cargo.lock
--rw-r--r--   0        0        0      248 1970-01-01 00:00:00.000000 quil-0.7.1rc0/Cargo.toml
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 quil-0.7.1rc0/pyproject.toml
--rw-r--r--   0     1001      127      283 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/py.typed
--rw-r--r--   0     1001      127      161 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/validation/__init__.py
--rw-r--r--   0     1001      127      439 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/validation/identifier.pyi
--rw-r--r--   0     1001      127       41 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/validation/identifier.py
--rw-r--r--   0     1001      127       39 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/validation/__init__.pyi
--rw-r--r--   0     1001      127       30 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/expression/__init__.py
--rw-r--r--   0     1001      127     7690 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/expression/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/__init__.pyi
--rw-r--r--   0     1001      127      124 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/instructions/__init__.py
--rw-r--r--   0     1001      127    91321 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/instructions/__init__.pyi
--rw-r--r--   0     1001      127      129 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/program/__init__.py
--rw-r--r--   0     1001      127    17921 2024-03-19 00:35:07.000000 quil-0.7.1rc0/quil/program/__init__.pyi
--rw-r--r--   0     1001      127      777 2024-03-19 00:35:07.000000 quil-0.7.1rc0/README-py.md
--rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 quil-0.7.1rc0/PKG-INFO
+-rw-r--r--   0     1001      127     1414 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/Cargo.toml
+-rw-r--r--   0     1001      127    43787 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/CHANGELOG.md
+-rw-r--r--   0     1001      127      954 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/README.md
+-rw-r--r--   0     1001      127     1692 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/corpus.rs
+-rw-r--r--   0     1001      127      941 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/get_frames_for_instruction.rs
+-rw-r--r--   0     1001      127      985 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/parser.rs
+-rw-r--r--   0     1001      127   803952 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/sample-calibrations.quil
+-rw-r--r--   0     1001      127     1478 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/scheduled_program_from_program.rs
+-rw-r--r--   0     1001      127      969 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/simplification.rs
+-rw-r--r--   0     1001      127    12979 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/benches/test_expressions.txt
+-rw-r--r--   0     1001      127     6316 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/examples/generate_test_expressions.rs
+-rw-r--r--   0     1001      127    38082 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/expression/mod.rs
+-rw-r--r--   0     1001      127    34338 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/expression/simplification/by_hand.rs
+-rw-r--r--   0     1001      127    12745 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/expression/simplification/mod.rs
+-rw-r--r--   0     1001      127     1002 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/hash.rs
+-rw-r--r--   0     1001      127     5302 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     6478 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127     9937 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     5260 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     6939 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9857 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/frame.rs
+-rw-r--r--   0     1001      127    43954 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/gate.rs
+-rw-r--r--   0     1001      127      771 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127    39423 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1798 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127     3425 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      654 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/reset.rs
+-rw-r--r--   0     1001      127      133 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Fixed Qubit.snap
+-rw-r--r--   0     1001      127      133 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__calibration__test_measure_calibration_definition__display@With Variable Qubit.snap
+-rw-r--r--   0     1001      127      124 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition No Params.snap
+-rw-r--r--   0     1001      127      167 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Params.snap
+-rw-r--r--   0     1001      127      160 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__circuit__test_circuit_definition__display@CircuitDefinition With Single Param.snap
+-rw-r--r--   0     1001      127      109 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Basic Declaration.snap
+-rw-r--r--   0     1001      127      141 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration with Offsets.snap
+-rw-r--r--   0     1001      127      125 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__declaration__test_declaration__display@Shared Declaration.snap
+-rw-r--r--   0     1001      127      191 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Parameterized GateDefinition.snap
+-rw-r--r--   0     1001      127      178 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Pauli Sum GateDefinition.snap
+-rw-r--r--   0     1001      127      139 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__gate__test_gate_definition__display@Permutation GateDefinition.snap
+-rw-r--r--   0     1001      127      143 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/snapshots/quil_rs__instruction__waveform__test_waveform_definition__display@Simple WaveformDefinition.snap
+-rw-r--r--   0     1001      127     1528 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     3619 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1910 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/lib.rs
+-rw-r--r--   0     1001      127     1013 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/macros.rs
+-rw-r--r--   0     1001      127    36217 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/command.rs
+-rw-r--r--   0     1001      127    23037 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/common.rs
+-rw-r--r--   0     1001      127     5970 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/error.rs
+-rw-r--r--   0     1001      127     2519 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/input.rs
+-rw-r--r--   0     1001      127     3242 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/internal.rs
+-rw-r--r--   0     1001      127     1004 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/kind.rs
+-rw-r--r--   0     1001      127     2685 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/error/mod.rs
+-rw-r--r--   0     1001      127    17487 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/expression.rs
+-rw-r--r--   0     1001      127     2212 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/gate.rs
+-rw-r--r--   0     1001      127    40956 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/instruction.rs
+-rw-r--r--   0     1001      127     1380 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/error.rs
+-rw-r--r--   0     1001      127    17439 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/mod.rs
+-rw-r--r--   0     1001      127     4222 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/quoted_strings.rs
+-rw-r--r--   0     1001      127     3357 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/lexer/wrapped_parsers.rs
+-rw-r--r--   0     1001      127     4162 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/macros.rs
+-rw-r--r--   0     1001      127     2446 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/mod.rs
+-rw-r--r--   0     1001      127     5841 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/parser/token.rs
+-rw-r--r--   0     1001      127    25985 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/control_flow_graph.rs
+-rw-r--r--   0     1001      127      974 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/mod.rs
+-rw-r--r--   0     1001      127     9591 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/qubit_graph.rs
+-rw-r--r--   0     1001      127      889 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap
+-rw-r--r--   0     1001      127     1329 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/analysis/test_programs.rs
+-rw-r--r--   0     1001      127    23626 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/calibration.rs
+-rw-r--r--   0     1001      127     8286 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/calibration_set.rs
+-rw-r--r--   0     1001      127     2283 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/leftover.rs
+-rw-r--r--   0     1001      127     3068 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/mod.rs
+-rw-r--r--   0     1001      127     2252 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/result.rs
+-rw-r--r--   0     1001      127     2725 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/error/syntax.rs
+-rw-r--r--   0     1001      127     8742 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/frame.rs
+-rw-r--r--   0     1001      127    17109 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/memory.rs
+-rw-r--r--   0     1001      127    48872 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/mod.rs
+-rw-r--r--   0     1001      127    26031 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/graph.rs
+-rw-r--r--   0     1001      127    20046 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/graphviz_dot.rs
+-rw-r--r--   0     1001      127      456 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/mod.rs
+-rw-r--r--   0     1001      127    16670 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/schedule.rs
+-rw-r--r--   0     1001      127     2678 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap
+-rw-r--r--   0     1001      127     1560 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap
+-rw-r--r--   0     1001      127     1166 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap
+-rw-r--r--   0     1001      127     1732 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap
+-rw-r--r--   0     1001      127     1112 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap
+-rw-r--r--   0     1001      127     1195 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap
+-rw-r--r--   0     1001      127     1780 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap
+-rw-r--r--   0     1001      127     1653 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap
+-rw-r--r--   0     1001      127     1003 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap
+-rw-r--r--   0     1001      127     1032 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap
+-rw-r--r--   0     1001      127      552 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap
+-rw-r--r--   0     1001      127     1540 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap
+-rw-r--r--   0     1001      127     1073 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap
+-rw-r--r--   0     1001      127     1338 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap
+-rw-r--r--   0     1001      127     1866 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap
+-rw-r--r--   0     1001      127      854 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap
+-rw-r--r--   0     1001      127      867 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap
+-rw-r--r--   0     1001      127      887 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap
+-rw-r--r--   0     1001      127     1892 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap
+-rw-r--r--   0     1001      127      839 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap
+-rw-r--r--   0     1001      127      768 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap
+-rw-r--r--   0     1001      127      591 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap
+-rw-r--r--   0     1001      127      793 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap
+-rw-r--r--   0     1001      127      852 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap
+-rw-r--r--   0     1001      127      585 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap
+-rw-r--r--   0     1001      127      227 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Instruction-Match.snap
+-rw-r--r--   0     1001      127      136 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Literal-Parameter.snap
+-rw-r--r--   0     1001      127      215 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Multiple-Qubits.snap
+-rw-r--r--   0     1001      127      476 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Param-Precedence.snap
+-rw-r--r--   0     1001      127      210 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Simple.snap
+-rw-r--r--   0     1001      127      141 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Calibration-Variable-Qubit.snap
+-rw-r--r--   0     1001      127      159 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@FenceVariableQubit.snap
+-rw-r--r--   0     1001      127      309 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Measure-Calibration.snap
+-rw-r--r--   0     1001      127      261 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Fixed-Match.snap
+-rw-r--r--   0     1001      127      155 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-No-Qubit-Match.snap
+-rw-r--r--   0     1001      127      254 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@Precedence-Variable-Match.snap
+-rw-r--r--   0     1001      127      174 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__calibration__tests__expansion@ShiftPhase.snap
+-rw-r--r--   0     1001      127      167 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__filter_instructions.snap
+-rw-r--r--   0     1001      127     3755 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap
+-rw-r--r--   0     1001      127      425 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__wrap_in_loop.snap
+-rw-r--r--   0     1001      127    35007 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/program/type_check.rs
+-rw-r--r--   0     1001      127     2422 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/quil.rs
+-rw-r--r--   0     1001      127     2749 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/reserved.rs
+-rw-r--r--   0     1001      127     2109 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/validation/identifier.rs
+-rw-r--r--   0     1001      127       20 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/src/validation/mod.rs
+-rw-r--r--   0     1001      127      724 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/calibration_test.rs
+-rw-r--r--   0     1001      127      742 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_cz.quil
+-rw-r--r--   0     1001      127     1888 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_cz_phase.quil
+-rw-r--r--   0     1001      127     3266 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_measure.quil
+-rw-r--r--   0     1001      127     1588 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_rx.quil
+-rw-r--r--   0     1001      127     1786 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/programs/calibration_xy.quil
+-rw-r--r--   0     1001      127      747 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap
+-rw-r--r--   0     1001      127     1797 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap
+-rw-r--r--   0     1001      127     3187 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap
+-rw-r--r--   0     1001      127     1519 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap
+-rw-r--r--   0     1001      127     1719 2024-04-15 17:47:41.000000 quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap
+-rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 quil-0.8.0/quil-py/Cargo.toml
+-rw-r--r--   0     1001      127      203 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/.flake8
+-rw-r--r--   0     1001      127       10 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/.stubtest-allowlist
+-rw-r--r--   0     1001      127    20226 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/CHANGELOG.md
+-rw-r--r--   0     1001      127      858 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/Makefile.toml
+-rw-r--r--   0     1001      127      777 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/README-py.md
+-rw-r--r--   0     1001      127      337 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/README.md
+-rw-r--r--   0     1001      127       71 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/build.rs
+-rw-r--r--   0     1001      127      404 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/make_docs.py
+-rw-r--r--   0     1001      127      135 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/index.html
+-rw-r--r--   0     1001      127    34673 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/quil/quil.html
+-rw-r--r--   0     1001      127    34581 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/quil.html
+-rw-r--r--   0     1001      127    20706 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/out/search.js
+-rw-r--r--   0     1001      127    36038 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/poetry.lock
+-rw-r--r--   0     1001      127      283 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/__init__.pyi
+-rw-r--r--   0     1001      127       30 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7690 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127      124 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91321 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127      129 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/program/__init__.py
+-rw-r--r--   0     1001      127    18326 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/py.typed
+-rw-r--r--   0     1001      127      161 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       39 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127       41 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/identifier.py
+-rw-r--r--   0     1001      127      439 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127    34593 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/quil.html
+-rw-r--r--   0     1001      127     6656 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/expression.rs
+-rw-r--r--   0     1001      127     2838 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/calibration.rs
+-rw-r--r--   0     1001      127     1251 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/circuit.rs
+-rw-r--r--   0     1001      127    11440 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/classical.rs
+-rw-r--r--   0     1001      127     4295 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/control_flow.rs
+-rw-r--r--   0     1001      127     5561 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/declaration.rs
+-rw-r--r--   0     1001      127     9528 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/frame.rs
+-rw-r--r--   0     1001      127     8394 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/gate.rs
+-rw-r--r--   0     1001      127     1056 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/measurement.rs
+-rw-r--r--   0     1001      127     8741 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/mod.rs
+-rw-r--r--   0     1001      127     1852 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/pragma.rs
+-rw-r--r--   0     1001      127      978 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/qubit.rs
+-rw-r--r--   0     1001      127      738 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/reset.rs
+-rw-r--r--   0     1001      127     1591 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/timing.rs
+-rw-r--r--   0     1001      127     2434 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/instruction/waveform.rs
+-rw-r--r--   0     1001      127     1967 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/lib.rs
+-rw-r--r--   0     1001      127     2701 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/analysis.rs
+-rw-r--r--   0     1001      127     4156 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/calibration.rs
+-rw-r--r--   0     1001      127     2774 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/frame.rs
+-rw-r--r--   0     1001      127      897 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/memory.rs
+-rw-r--r--   0     1001      127    12662 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/mod.rs
+-rw-r--r--   0     1001      127     1696 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/program/scheduling.rs
+-rw-r--r--   0     1001      127     1136 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/validation/identifier.rs
+-rw-r--r--   0     1001      127      151 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/src/validation/mod.rs
+-rw-r--r--   0     1001      127     1665 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/instructions/test_copy.py
+-rw-r--r--   0     1001      127      351 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/instructions/test_gate.py
+-rw-r--r--   0     1001      127      137 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/program/__snapshots__/test_program.ambr
+-rw-r--r--   0     1001      127     4566 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/program/test_program.py
+-rw-r--r--   0     1001      127     1023 2024-04-15 17:47:41.000000 quil-0.8.0/quil-py/test/test_eq.py
+-rw-r--r--   0     1001      127    50010 2024-04-15 17:47:41.000000 quil-0.8.0/Cargo.lock
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 quil-0.8.0/Cargo.toml
+-rw-r--r--   0        0        0     1575 1970-01-01 00:00:00.000000 quil-0.8.0/pyproject.toml
+-rw-r--r--   0     1001      127      124 2024-04-15 17:47:41.000000 quil-0.8.0/quil/instructions/__init__.py
+-rw-r--r--   0     1001      127    91321 2024-04-15 17:47:41.000000 quil-0.8.0/quil/instructions/__init__.pyi
+-rw-r--r--   0     1001      127      129 2024-04-15 17:47:41.000000 quil-0.8.0/quil/program/__init__.py
+-rw-r--r--   0     1001      127    18326 2024-04-15 17:47:41.000000 quil-0.8.0/quil/program/__init__.pyi
+-rw-r--r--   0     1001      127      439 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/identifier.pyi
+-rw-r--r--   0     1001      127      161 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/__init__.py
+-rw-r--r--   0     1001      127       41 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/identifier.py
+-rw-r--r--   0     1001      127       39 2024-04-15 17:47:41.000000 quil-0.8.0/quil/validation/__init__.pyi
+-rw-r--r--   0     1001      127      283 2024-04-15 17:47:41.000000 quil-0.8.0/quil/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil/py.typed
+-rw-r--r--   0     1001      127       30 2024-04-15 17:47:41.000000 quil-0.8.0/quil/expression/__init__.py
+-rw-r--r--   0     1001      127     7690 2024-04-15 17:47:41.000000 quil-0.8.0/quil/expression/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-15 17:47:41.000000 quil-0.8.0/quil/__init__.pyi
+-rw-r--r--   0     1001      127      777 2024-04-15 17:47:41.000000 quil-0.8.0/README-py.md
+-rw-r--r--   0        0        0     1467 1970-01-01 00:00:00.000000 quil-0.8.0/PKG-INFO
```

### Comparing `quil-0.7.1rc0/quil-rs/Cargo.toml` & `quil-0.8.0/quil-rs/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [package]
 name = "quil-rs"
 description = "Rust tooling for Quil (Quantum Instruction Language)"
-version = "0.23.0"
+version = "0.24.0"
 edition = "2021"
 rust-version = "1.70"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rust"
 keywords = ["Quil", "Quantum", "Rigetti"]
 categories = ["parser-implementations", "science", "compilers", "emulators"]
 
 [dependencies]
 approx = { version = "0.5.1", features = ["num-complex"] }
 dot-writer = { version = "0.1.2", optional = true }
-indexmap = "2.2.2"
 itertools = "0.12.1"
 lexical = "6.1.1"
 ndarray.workspace = true
 nom = "7.1.1"
 nom_locate = "4.0.0"
 num-complex = "0.4.0"
 once_cell = "1.17.1"
 petgraph = "0.6.4"
 regex = "1.7.1"
 serde = { version = "1.0.125", features = ["derive"] }
 strum.workspace = true
 thiserror = "1.0.56"
+indexmap.workspace = true
 
 [dev-dependencies]
 clap = { version = "4.3.19", features = ["derive", "string"] }
 criterion = { version = "0.5.1", features = ["html_reports"] }
-insta = "1.7.1"
+insta = "1.37.0"
 petgraph = "0.6.2"
 proptest = "1.0.0"
 proptest-derive = "0.3.0"
 rand = "0.8.5"
 rstest = "0.18.2"
 
 # These are described in the crate README.md
```

### Comparing `quil-0.7.1rc0/quil-rs/CHANGELOG.md` & `quil-0.8.0/quil-rs/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## 0.24.0
+
+### Breaking Changes
+
+- CalibrationSet's and Program's will be considered equal if they contain the same set of calibrations, regardless of order. (#352)
+
+## 0.24.0-rc.0
+
+### Breaking Changes
+
+- CalibrationSet's and Program's will be considered equal if they contain the same set of calibrations, regardless of order. (#352)
+
 ## 0.23.0
 
 ### Breaking Changes
 
 - #334: program scheduling and analysis utilities (#336)
 
 ### Fixes
```

### Comparing `quil-0.7.1rc0/quil-rs/README.md` & `quil-0.8.0/quil-rs/README.md`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/benches/corpus.rs` & `quil-0.8.0/quil-rs/benches/corpus.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/benches/get_frames_for_instruction.rs` & `quil-0.8.0/quil-rs/benches/get_frames_for_instruction.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/benches/parser.rs` & `quil-0.8.0/quil-rs/benches/parser.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/benches/sample-calibrations.quil` & `quil-0.8.0/quil-rs/benches/sample-calibrations.quil`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/benches/scheduled_program_from_program.rs` & `quil-0.8.0/quil-rs/benches/scheduled_program_from_program.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/benches/simplification.rs` & `quil-0.8.0/quil-rs/benches/simplification.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/benches/test_expressions.txt` & `quil-0.8.0/quil-rs/benches/test_expressions.txt`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/examples/generate_test_expressions.rs` & `quil-0.8.0/quil-rs/examples/generate_test_expressions.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/expression/mod.rs` & `quil-0.8.0/quil-rs/src/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/expression/simplification/by_hand.rs` & `quil-0.8.0/quil-rs/src/expression/simplification/by_hand.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/expression/simplification/mod.rs` & `quil-0.8.0/quil-rs/src/expression/simplification/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/hash.rs` & `quil-0.8.0/quil-rs/src/hash.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/circuit.rs` & `quil-0.8.0/quil-rs/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/classical.rs` & `quil-0.8.0/quil-rs/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/control_flow.rs` & `quil-0.8.0/quil-rs/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/declaration.rs` & `quil-0.8.0/quil-rs/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/frame.rs` & `quil-0.8.0/quil-rs/src/instruction/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/gate.rs` & `quil-0.8.0/quil-rs/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/measurement.rs` & `quil-0.8.0/quil-rs/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/mod.rs` & `quil-0.8.0/quil-rs/src/instruction/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 mod measurement;
 mod pragma;
 mod qubit;
 mod reset;
 mod timing;
 mod waveform;
 
-pub use self::calibration::{Calibration, MeasureCalibrationDefinition};
+pub use self::calibration::{Calibration, CalibrationSignature, MeasureCalibrationDefinition};
 pub use self::circuit::CircuitDefinition;
 pub use self::classical::{
     Arithmetic, ArithmeticOperand, ArithmeticOperator, BinaryLogic, BinaryOperand, BinaryOperands,
     BinaryOperator, Comparison, ComparisonOperand, ComparisonOperator, Convert, Exchange, Move,
     UnaryLogic, UnaryOperator,
 };
 pub use self::control_flow::{Jump, JumpUnless, JumpWhen, Label, Target, TargetPlaceholder};
```

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/pragma.rs` & `quil-0.8.0/quil-rs/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/qubit.rs` & `quil-0.8.0/quil-rs/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/reset.rs` & `quil-0.8.0/quil-rs/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/timing.rs` & `quil-0.8.0/quil-rs/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/instruction/waveform.rs` & `quil-0.8.0/quil-rs/src/instruction/waveform.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/lib.rs` & `quil-0.8.0/quil-rs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/macros.rs` & `quil-0.8.0/quil-rs/src/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/command.rs` & `quil-0.8.0/quil-rs/src/parser/command.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/common.rs` & `quil-0.8.0/quil-rs/src/parser/common.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/error/error.rs` & `quil-0.8.0/quil-rs/src/parser/error/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/error/input.rs` & `quil-0.8.0/quil-rs/src/parser/error/input.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/error/internal.rs` & `quil-0.8.0/quil-rs/src/parser/error/internal.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/error/kind.rs` & `quil-0.8.0/quil-rs/src/parser/error/kind.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/error/mod.rs` & `quil-0.8.0/quil-rs/src/parser/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/expression.rs` & `quil-0.8.0/quil-rs/src/parser/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/gate.rs` & `quil-0.8.0/quil-rs/src/parser/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/instruction.rs` & `quil-0.8.0/quil-rs/src/parser/instruction.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/lexer/error.rs` & `quil-0.8.0/quil-rs/src/parser/lexer/error.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/lexer/mod.rs` & `quil-0.8.0/quil-rs/src/parser/lexer/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/lexer/quoted_strings.rs` & `quil-0.8.0/quil-rs/src/parser/lexer/quoted_strings.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/lexer/wrapped_parsers.rs` & `quil-0.8.0/quil-rs/src/parser/lexer/wrapped_parsers.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/macros.rs` & `quil-0.8.0/quil-rs/src/parser/macros.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/mod.rs` & `quil-0.8.0/quil-rs/src/parser/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/parser/token.rs` & `quil-0.8.0/quil-rs/src/parser/token.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/analysis/control_flow_graph.rs` & `quil-0.8.0/quil-rs/src/program/analysis/control_flow_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/analysis/mod.rs` & `quil-0.8.0/quil-rs/src/program/analysis/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/analysis/qubit_graph.rs` & `quil-0.8.0/quil-rs/src/program/analysis/qubit_graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap` & `quil-0.8.0/quil-rs/src/program/analysis/snapshots/quil_rs__program__analysis__control_flow_graph__tests__schedule_uncalibrated_cz.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/analysis/test_programs.rs` & `quil-0.8.0/quil-rs/src/program/analysis/test_programs.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/calibration.rs` & `quil-0.8.0/quil-rs/src/program/calibration.rs`

 * *Files 16% similar despite different names*

```diff
@@ -13,32 +13,31 @@
 // limitations under the License.
 
 use std::collections::HashMap;
 
 use itertools::FoldWhile::{Continue, Done};
 use itertools::Itertools;
 
-use crate::instruction::Fence;
 use crate::quil::Quil;
 use crate::{
     expression::Expression,
     instruction::{
-        Calibration, Capture, Delay, FrameIdentifier, Gate, Instruction,
+        Calibration, Capture, Delay, Fence, FrameIdentifier, Gate, Instruction,
         MeasureCalibrationDefinition, Measurement, Pulse, Qubit, RawCapture, SetFrequency,
         SetPhase, SetScale, ShiftFrequency, ShiftPhase,
     },
 };
 
-use super::ProgramError;
+use super::{CalibrationSet, ProgramError};
 
 /// A collection of Quil calibrations (`DEFCAL` instructions) with utility methods.
 #[derive(Clone, Debug, Default, PartialEq)]
-pub struct CalibrationSet {
-    pub calibrations: Vec<Calibration>,
-    pub measure_calibrations: Vec<MeasureCalibrationDefinition>,
+pub struct Calibrations {
+    pub calibrations: CalibrationSet<Calibration>,
+    pub measure_calibrations: CalibrationSet<MeasureCalibrationDefinition>,
 }
 
 struct MatchedCalibration<'a> {
     pub calibration: &'a Calibration,
     pub fixed_qubit_count: usize,
 }
 
@@ -54,23 +53,34 @@
                     Qubit::Placeholder(_) | Qubit::Variable(_) => false,
                 })
                 .count(),
         }
     }
 }
 
-impl CalibrationSet {
-    /// Return all [`Calibration`]s in the set
-    pub fn calibrations(&self) -> &[Calibration] {
-        self.calibrations.as_ref()
+impl Calibrations {
+    /// Return a vector containing a reference to all [`Calibration`]s in the set.
+    pub fn calibrations(&self) -> Vec<&Calibration> {
+        self.iter_calibrations().collect()
     }
 
-    /// Return all [`MeasureCalibrationDefinition`]s in the set
-    pub fn measure_calibrations(&self) -> &[MeasureCalibrationDefinition] {
-        self.measure_calibrations.as_ref()
+    /// Return a vector containing a reference to all [`MeasureCalibrationDefinition`]s
+    /// in the set.
+    pub fn measure_calibrations(&self) -> Vec<&MeasureCalibrationDefinition> {
+        self.iter_measure_calibrations().collect()
+    }
+
+    /// Iterate over all [`Calibration`]s in the set
+    pub fn iter_calibrations(&self) -> impl Iterator<Item = &Calibration> {
+        self.calibrations.iter()
+    }
+
+    /// Iterate over all [`MeasureCalibrationDefinition`]s calibrations in the set
+    pub fn iter_measure_calibrations(&self) -> impl Iterator<Item = &MeasureCalibrationDefinition> {
+        self.measure_calibrations.iter()
     }
 
     /// Given an instruction, return the instructions to which it is expanded if there is a match.
     /// Recursively calibrate instructions, returning an error if a calibration directly or indirectly
     /// expands into itself.
     pub fn expand(
         &self,
@@ -247,15 +257,15 @@
     pub fn get_match_for_measurement(
         &self,
         measurement: &Measurement,
     ) -> Option<&MeasureCalibrationDefinition> {
         measurement.target.as_ref()?;
 
         self.measure_calibrations()
-            .iter()
+            .into_iter()
             .rev()
             .fold_while(None, |best_match, calibration| {
                 if let Some(qubit) = &calibration.qubit {
                     match qubit {
                         Qubit::Fixed(_) if qubit == &measurement.qubit => Done(Some(calibration)),
                         Qubit::Variable(_)
                             if best_match.is_none()
@@ -282,15 +292,15 @@
     /// 3. It has the same qubit count (any mix of fixed & variable)
     /// 4. It has the same parameter count (both specified and unspecified)
     /// 5. All fixed qubits in the calibration definition match those in the gate
     /// 6. All specified parameters in the calibration definition match those in the gate
     pub fn get_match_for_gate(&self, gate: &Gate) -> Option<&Calibration> {
         let mut matched_calibration: Option<MatchedCalibration> = None;
 
-        for calibration in &self.calibrations {
+        for calibration in self.iter_calibrations() {
             // Filter out non-matching calibrations: check rules 1-4
             if calibration.name != gate.name
                 || calibration.modifiers != gate.modifiers
                 || calibration.parameters.len() != gate.parameters.len()
                 || calibration.qubits.len() != gate.qubits.len()
             {
                 continue;
@@ -367,59 +377,63 @@
     }
 
     /// Return true if this contains no data.
     pub fn is_empty(&self) -> bool {
         self.calibrations.is_empty()
     }
 
-    /// Add another gate calibration to the set.
-    /// Deprecated in favor of [`Self::push_calibration`]
-    #[deprecated = "use ScheduledProgram#push_calibration instead"]
-    pub fn push(&mut self, calibration: Calibration) {
-        self.push_calibration(calibration)
-    }
-
-    /// Add another gate calibration (`DEFCAL`) to the set.
-    pub fn push_calibration(&mut self, calibration: Calibration) {
-        self.calibrations.push(calibration)
+    /// Insert a [`Calibration`] into the set.
+    ///
+    /// If a calibration with the same [`CalibrationSignature`] already exists in the set, it will
+    /// be replaced, and the old calibration is returned.
+    pub fn insert_calibration(&mut self, calibration: Calibration) -> Option<Calibration> {
+        self.calibrations.replace(calibration)
     }
 
-    /// Add another measurement calibration (`DEFCAL MEASURE`) to the set.
-    pub fn push_measurement_calibration(&mut self, calibration: MeasureCalibrationDefinition) {
-        self.measure_calibrations.push(calibration)
+    /// Insert a [`MeasureCalibration`] into the set.
+    ///
+    /// If a calibration with the same [`CalibrationSignature`] already exists in the set, it will
+    /// be replaced, and the old calibration is returned.
+    pub fn insert_measurement_calibration(
+        &mut self,
+        calibration: MeasureCalibrationDefinition,
+    ) -> Option<MeasureCalibrationDefinition> {
+        self.measure_calibrations.replace(calibration)
     }
 
-    /// Append another [`CalibrationSet`] onto this one
-    pub fn extend(&mut self, other: CalibrationSet) {
+    /// Append another [`CalibrationSet`] onto this one.
+    ///
+    /// Calibrations with conflicting [`CalibrationSignature`]s are overwritten by the ones in the
+    /// given set.
+    pub fn extend(&mut self, other: Calibrations) {
         self.calibrations.extend(other.calibrations);
         self.measure_calibrations.extend(other.measure_calibrations);
     }
 
-    /// Return the Quil instructions which describe the contained calibrations, consuming the [`CalibrationSet`].
+    /// Return the Quil instructions which describe the contained calibrations, consuming the
+    /// [`CalibrationSet`]
     pub fn into_instructions(self) -> Vec<Instruction> {
         self.calibrations
             .into_iter()
             .map(Instruction::CalibrationDefinition)
             .chain(
                 self.measure_calibrations
                     .into_iter()
                     .map(Instruction::MeasureCalibrationDefinition),
             )
             .collect()
     }
 
     /// Return the Quil instructions which describe the contained calibrations.
     pub fn to_instructions(&self) -> Vec<Instruction> {
-        self.calibrations
-            .iter()
+        self.iter_calibrations()
             .cloned()
             .map(Instruction::CalibrationDefinition)
             .chain(
-                self.measure_calibrations
-                    .iter()
+                self.iter_measure_calibrations()
                     .cloned()
                     .map(Instruction::MeasureCalibrationDefinition),
             )
             .collect()
     }
 }
```

### Comparing `quil-0.7.1rc0/quil-rs/src/program/error/leftover.rs` & `quil-0.8.0/quil-rs/src/program/error/leftover.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/error/mod.rs` & `quil-0.8.0/quil-rs/src/program/error/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/error/result.rs` & `quil-0.8.0/quil-rs/src/program/error/result.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/error/syntax.rs` & `quil-0.8.0/quil-rs/src/program/error/syntax.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/frame.rs` & `quil-0.8.0/quil-rs/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/memory.rs` & `quil-0.8.0/quil-rs/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/mod.rs` & `quil-0.8.0/quil-rs/src/program/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -25,22 +25,24 @@
     FrameIdentifier, GateDefinition, GateError, Instruction, Jump, JumpUnless, Label, Matrix,
     MemoryReference, Move, Qubit, QubitPlaceholder, ScalarType, Target, TargetPlaceholder, Vector,
     Waveform, WaveformDefinition,
 };
 use crate::parser::{lex, parse_instructions, ParseError};
 use crate::quil::Quil;
 
-pub use self::calibration::CalibrationSet;
+pub use self::calibration::Calibrations;
+pub use self::calibration_set::CalibrationSet;
 pub use self::error::{disallow_leftover, map_parsed, recover, ParseProgramError, SyntaxError};
 pub use self::frame::FrameSet;
 pub use self::frame::MatchedFrames;
 pub use self::memory::{MemoryAccesses, MemoryRegion};
 
 pub mod analysis;
 mod calibration;
+mod calibration_set;
 mod error;
 pub(crate) mod frame;
 mod memory;
 pub mod scheduling;
 pub mod type_check;
 
 #[derive(Debug, thiserror::Error, PartialEq)]
@@ -66,28 +68,28 @@
 /// A Quil Program instance describes a quantum program with metadata used in execution.
 ///
 /// This contains not only instructions which are executed in turn on the quantum processor, but
 /// also the "headers" used to describe and manipulate those instructions, such as calibrations
 /// and frame definitions.
 #[derive(Clone, Debug, Default, PartialEq)]
 pub struct Program {
-    pub calibrations: CalibrationSet,
+    pub calibrations: Calibrations,
     pub frames: FrameSet,
     pub memory_regions: BTreeMap<String, MemoryRegion>,
     pub waveforms: BTreeMap<String, Waveform>,
     pub gate_definitions: BTreeMap<String, GateDefinition>,
     instructions: Vec<Instruction>,
     // private field used for caching operations
     used_qubits: HashSet<Qubit>,
 }
 
 impl Program {
     pub fn new() -> Self {
         Program {
-            calibrations: CalibrationSet::default(),
+            calibrations: Calibrations::default(),
             frames: FrameSet::new(),
             memory_regions: BTreeMap::new(),
             waveforms: BTreeMap::new(),
             gate_definitions: BTreeMap::new(),
             instructions: vec![],
             used_qubits: HashSet::new(),
         }
@@ -132,15 +134,15 @@
     /// Add an instruction to the end of the program.
     pub fn add_instruction(&mut self, instruction: Instruction) {
         self.used_qubits
             .extend(instruction.get_qubits().into_iter().cloned());
 
         match instruction {
             Instruction::CalibrationDefinition(calibration) => {
-                self.calibrations.push_calibration(calibration);
+                self.calibrations.insert_calibration(calibration);
             }
             Instruction::FrameDefinition(FrameDefinition {
                 identifier,
                 attributes,
             }) => {
                 self.frames.insert(identifier, attributes);
             }
@@ -153,15 +155,16 @@
                     .insert(name, MemoryRegion { size, sharing });
             }
             Instruction::GateDefinition(gate_definition) => {
                 self.gate_definitions
                     .insert(gate_definition.name.clone(), gate_definition);
             }
             Instruction::MeasureCalibrationDefinition(calibration) => {
-                self.calibrations.push_measurement_calibration(calibration);
+                self.calibrations
+                    .insert_measurement_calibration(calibration);
             }
             Instruction::WaveformDefinition(WaveformDefinition { name, definition }) => {
                 self.waveforms.insert(name, definition);
             }
             Instruction::Gate(gate) => {
                 self.instructions.push(Instruction::Gate(gate));
             }
@@ -332,15 +335,15 @@
                 sharing: descriptor.sharing,
             })
         }));
         instructions.extend(self.frames.into_instructions());
         instructions.extend(self.waveforms.into_iter().map(|(name, definition)| {
             Instruction::WaveformDefinition(WaveformDefinition { name, definition })
         }));
-        instructions.extend(self.calibrations.into_instructions());
+        instructions.extend(self.calibrations.to_instructions());
         instructions.extend(
             self.gate_definitions
                 .into_values()
                 .map(Instruction::GateDefinition),
         );
         instructions.extend(self.instructions);
         instructions
@@ -356,15 +359,15 @@
     ///
     /// When a valid program is simplified, it remains valid.
     pub fn into_simplified(&self) -> Result<Self> {
         let mut expanded_program = self.expand_calibrations()?;
         // Remove calibrations such that the resulting program contains
         // only instructions. Calibrations have already been expanded, so
         // technically there is no need to keep them around anyway.
-        expanded_program.calibrations = CalibrationSet::default();
+        expanded_program.calibrations = Calibrations::default();
 
         let mut frames_used: HashSet<&FrameIdentifier> = HashSet::new();
         let mut waveforms_used: HashSet<&String> = HashSet::new();
 
         for instruction in &expanded_program.instructions {
             if let Some(matched_frames) = expanded_program.get_frames_for_instruction(instruction) {
                 frames_used.extend(matched_frames.used())
@@ -998,15 +1001,15 @@
 DEFFRAME 0 \"rx\":
     HARDWARE-OBJECT: \"hardware\"
 DEFWAVEFORM custom:
     1,2
 I 0
 ";
         let program = Program::from_str(input).unwrap();
-        let expected_owned = vec![Qubit::Fixed(0), Qubit::Variable("q".to_string())];
+        let expected_owned = [Qubit::Fixed(0), Qubit::Variable("q".to_string())];
         let expected = expected_owned.iter().collect::<HashSet<_>>();
         let actual = program.get_used_qubits();
         assert_eq!(expected, actual.iter().collect());
     }
 
     #[test]
     fn test_add_instructions() {
@@ -1053,15 +1056,15 @@
         let lhs = Program::from_str(lhs_input).unwrap();
         let rhs = Program::from_str(rhs_input).unwrap();
 
         let sum = lhs.clone() + rhs.clone();
         let mut in_place_sum = lhs.clone();
         in_place_sum += rhs;
 
-        let expected_qubits = vec![
+        let expected_qubits = [
             Qubit::Fixed(0),
             Qubit::Fixed(1),
             Qubit::Fixed(2),
             Qubit::Fixed(3),
             Qubit::Variable("q".to_string()),
         ];
 
@@ -1351,8 +1354,68 @@
             Target::Fixed("loop-start".to_string()),
             Target::Fixed("loop-end".to_string()),
             10,
         );
 
         assert_snapshot!(program.to_quil().unwrap())
     }
+
+    #[test]
+    fn test_equality() {
+        let input = "DECLARE foo REAL[1]
+DEFFRAME 1 \"rx\":
+\tHARDWARE-OBJECT: \"hardware\"
+DEFCAL I 0:
+\tDELAY 0 1
+DEFCAL I 1:
+\tDELAY 0 1
+DEFCAL I 2:
+\tDELAY 0 1
+DEFCAL MEASURE 0 addr:
+\tCAPTURE 0 \"ro_rx\" custom addr
+DEFCAL MEASURE 1 addr:
+\tCAPTURE 1 \"ro_rx\" custom addr
+DEFWAVEFORM custom:
+\t1,2
+DEFWAVEFORM custom2:
+\t3,4
+DEFWAVEFORM another1:
+\t4,5
+DEFGATE BAR AS MATRIX:
+\t0, 1
+\t1, 0
+DEFGATE FOO AS MATRIX:
+\t0, 1
+\t1, 0
+
+H 1
+CNOT 2 3";
+
+        let program = Program::from_str(input).unwrap();
+
+        // The order of definitions are global in the sense that where they are defined in a
+        // program does not matter.
+        let is_global_state_instruction = move |i: &Instruction| -> bool {
+            matches!(
+                i,
+                Instruction::CalibrationDefinition(_)
+                    | Instruction::MeasureCalibrationDefinition(_)
+                    | Instruction::WaveformDefinition(_)
+                    | Instruction::GateDefinition(_)
+                    | Instruction::FrameDefinition(_)
+            )
+        };
+        // Create a copy of the program, but insert the "global" instructions in reverse order.
+        // Since where these instructions are defined doesn't matter, this should be an
+        // equivalent program.
+        let mut program2 = program.filter_instructions(|i| !is_global_state_instruction(i));
+        let global_instructions: Vec<Instruction> = program
+            .filter_instructions(is_global_state_instruction)
+            .into_instructions()
+            .into_iter()
+            .rev()
+            .collect();
+        program2.add_instructions(global_instructions);
+
+        assert_eq!(program, program2);
+    }
 }
```

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/graph.rs` & `quil-0.8.0/quil-rs/src/program/scheduling/graph.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/graphviz_dot.rs` & `quil-0.8.0/quil-rs/src/program/scheduling/graphviz_dot.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/schedule.rs` & `quil-0.8.0/quil-rs/src/program/scheduling/schedule.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__mixed_pragmas_and_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_with_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graph__tests__custom_handler__only_pragmas_without_frames.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__active_reset_single_frame.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_2q_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_after_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__blocking_pulses_wrap_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__chained_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_blocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__different_frames_nonblocking.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_all_with_nonblocking_pulses.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_one_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__fence_wrapper.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__jump.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__labels_only.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__multiple_classical_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulse.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__parametric_pulses_using_capture_results.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__pulse_after_set_frequency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_capture.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__simple_memory_access.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_dependency.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap` & `quil-0.8.0/quil-rs/src/program/scheduling/snapshots/quil_rs__program__scheduling__graphviz_dot__tests__graph__single_instruction.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap` & `quil-0.8.0/quil-rs/src/program/snapshots/quil_rs__program__tests__to_instructions.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/program/type_check.rs` & `quil-0.8.0/quil-rs/src/program/type_check.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/quil.rs` & `quil-0.8.0/quil-rs/src/quil.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/src/reserved.rs` & `quil-0.8.0/quil-rs/src/reserved.rs`

 * *Files 7% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 #[derive(Clone, Debug, PartialEq, Eq)]
 pub enum ReservedToken {
     Keyword(ReservedKeyword),
     Gate(ReservedGate),
     Constant(ReservedConstant),
 }
 
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, thiserror::Error)]
+#[error("{0} is not a reserved token")]
 pub struct NotReservedToken(String);
 
 impl FromStr for ReservedToken {
     type Err = NotReservedToken;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         if let Ok(keyword) = ReservedKeyword::from_str(s) {
             Ok(Self::Keyword(keyword))
         } else if let Ok(gate) = ReservedGate::from_str(s) {
             Ok(Self::Gate(gate))
         } else if let Ok(constant) = ReservedConstant::from_str(s) {
             Ok(Self::Constant(constant))
         } else {
-            Err(NotReservedToken(format!("{s} is not a reserved token")))
+            Err(NotReservedToken(s.to_string()))
         }
     }
 }
 
 impl Display for ReservedToken {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         match self {
```

### Comparing `quil-0.7.1rc0/quil-rs/src/validation/identifier.rs` & `quil-0.8.0/quil-rs/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/calibration_test.rs` & `quil-0.8.0/quil-rs/tests/calibration_test.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/programs/calibration_cz.quil` & `quil-0.8.0/quil-rs/tests/programs/calibration_cz.quil`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/programs/calibration_cz_phase.quil` & `quil-0.8.0/quil-rs/tests/programs/calibration_cz_phase.quil`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/programs/calibration_measure.quil` & `quil-0.8.0/quil-rs/tests/programs/calibration_measure.quil`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/programs/calibration_rx.quil` & `quil-0.8.0/quil-rs/tests/programs/calibration_rx.quil`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/programs/calibration_xy.quil` & `quil-0.8.0/quil-rs/tests/programs/calibration_xy.quil`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap` & `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap` & `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_cz_phase.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap` & `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_measure.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap` & `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_rx.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap` & `quil-0.8.0/quil-rs/tests/snapshots/calibration_test__calibration_xy.quil.snap`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/Cargo.toml` & `quil-0.8.0/quil-py/Cargo.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "quil-py"
 description = "Python bindings for quil-rs"
-version = "0.7.1-rc.0"
+version = "0.8.0"
 edition = "2021"
 license = "Apache-2.0"
 repository = "https://github.com/rigetti/quil-rs"
 keywords = ["pyquil", "SDK", "Rigetti", "Quil", "Quantum"]
 categories = ["api-bindings", "parsers", "science", "emulators"]
 readme = "./README.md"
 
@@ -18,16 +18,17 @@
 #
 # Downstream Rust code (including code in `bin/`, `examples/`, and `tests/`) will not be able
 # to `use quil;` unless the "lib" and "rlib" crate type is also included:
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
 ndarray.workspace = true
-quil-rs = { path = "../quil-rs", version = "0.23.0" }
+quil-rs = { path = "../quil-rs", version = "0.24.0" }
 strum.workspace = true
 # pyo3 dependencies should be updated together
 numpy = "0.20.0"
-pyo3 = "0.20.0"
+pyo3 = { version = "0.20.3", features = ["indexmap"] }
 rigetti-pyo3 = "0.3.1"
+indexmap.workspace = true
 
 [build-dependencies]
 pyo3-build-config = "0.20.0"
```

### Comparing `quil-0.7.1rc0/quil-py/CHANGELOG.md` & `quil-0.8.0/quil-py/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+## 0.8.0
+
+### Breaking Changes
+
+- CalibrationSet's and Program's will be considered equal if they contain the same set of calibrations, regardless of order. (#352)
+
+## 0.8.0-rc.0
+
+### Breaking Changes
+
+- CalibrationSet's and Program's will be considered equal if they contain the same set of calibrations, regardless of order. (#352)
+
+## 0.7.1
+
+### Features
+
+- linux ppc64le wheel
+
 ## 0.7.1-rc.0
 
 ### Features
 
 - linux ppc64le wheel
 
 ## 0.7.0
```

### Comparing `quil-0.7.1rc0/quil-py/Makefile.toml` & `quil-0.8.0/quil-py/Makefile.toml`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/README-py.md` & `quil-0.8.0/quil-py/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/out/quil/quil.html` & `quil-0.8.0/quil-py/out/quil/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/out/quil.html` & `quil-0.8.0/quil-py/out/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/out/search.js` & `quil-0.8.0/quil-py/out/search.js`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/poetry.lock` & `quil-0.8.0/quil-py/poetry.lock`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/quil/expression/__init__.pyi` & `quil-0.8.0/quil-py/quil/expression/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/quil/instructions/__init__.pyi` & `quil-0.8.0/quil-py/quil/instructions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/quil/program/__init__.pyi` & `quil-0.8.0/quil-py/quil/program/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -318,22 +318,28 @@
         5. All fixed qubits in the calibration definition match those in the gate
         6. All specified parameters in the calibration definition match those in the gate
         """
     def __len__(self) -> int: ...
     def is_empty(self) -> bool:
         """Returns ``True`` if the ``CalibrationSet`` contains no data."""
         ...
-    def push_calibration(self, calibration: Calibration):
+    def insert_calibration(self, calibration: Calibration) -> Optional[Calibration]:
         """
-        Add another gate ``Calibration`` (`DEFCAL`) to the set.
+        Insert another ``Calibration`` (`DEFCAL`) to the set.
+
+        If a calibration with the same name already exists, it is overwritten and this
+        function returns the previous calibration. Otherwise, None is returned.
         """
         ...
-    def push_measurement_calibration(self, calibration: MeasureCalibrationDefinition):
+    def insert_measurement_calibration(self, calibration: MeasureCalibrationDefinition) -> Optional[MeasureCalibrationDefinition]:
         """
         Add another ``MeasureCalibrationDefinition`` (`DEFCAL MEASURE`) to the set
+
+        If a calibration with the same name already exists, it is overwritten and this
+        function returns the previous calibration. Otherwise, None is returned.
         """
     def extend(self, other: CalibrationSet):
         """
         Append another [`CalibrationSet`] onto this one
         """
         ...
     def to_instructions(self):
```

### Comparing `quil-0.7.1rc0/quil-py/quil.html` & `quil-0.8.0/quil-py/quil.html`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/expression.rs` & `quil-0.8.0/quil-py/src/expression.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/calibration.rs` & `quil-0.8.0/quil-py/src/instruction/calibration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/circuit.rs` & `quil-0.8.0/quil-py/src/instruction/circuit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/classical.rs` & `quil-0.8.0/quil-py/src/instruction/classical.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/control_flow.rs` & `quil-0.8.0/quil-py/src/instruction/control_flow.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/declaration.rs` & `quil-0.8.0/quil-py/src/instruction/declaration.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/frame.rs` & `quil-0.8.0/quil-py/src/instruction/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/gate.rs` & `quil-0.8.0/quil-py/src/instruction/gate.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/measurement.rs` & `quil-0.8.0/quil-py/src/instruction/measurement.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/mod.rs` & `quil-0.8.0/quil-py/src/instruction/mod.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/pragma.rs` & `quil-0.8.0/quil-py/src/instruction/pragma.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/qubit.rs` & `quil-0.8.0/quil-py/src/instruction/qubit.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/reset.rs` & `quil-0.8.0/quil-py/src/instruction/reset.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/timing.rs` & `quil-0.8.0/quil-py/src/instruction/timing.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/instruction/waveform.rs` & `quil-0.8.0/quil-py/src/instruction/waveform.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/lib.rs` & `quil-0.8.0/quil-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/program/analysis.rs` & `quil-0.8.0/quil-py/src/program/analysis.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/program/calibration.rs` & `quil-0.8.0/quil-py/src/program/calibration.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use quil_rs::{
     instruction::{Calibration, Gate, Instruction, MeasureCalibrationDefinition, Measurement},
-    program::CalibrationSet,
+    program::Calibrations,
 };
 use rigetti_pyo3::{
     impl_as_mut_for_wrapper, impl_repr, py_wrap_type,
     pyo3::{pymethods, PyResult, Python},
     PyTryFrom, PyWrapper, PyWrapperMut, ToPython, ToPythonError,
 };
 
@@ -15,31 +15,38 @@
     },
 };
 
 use super::ProgramError;
 
 py_wrap_type! {
     #[derive(Debug, PartialEq)]
-    PyCalibrationSet(CalibrationSet) as "CalibrationSet"
+    PyCalibrationSet(Calibrations) as "CalibrationSet"
 }
 impl_as_mut_for_wrapper!(PyCalibrationSet);
 impl_repr!(PyCalibrationSet);
 impl_eq!(PyCalibrationSet);
 
 #[pymethods]
 impl PyCalibrationSet {
     #[new]
     pub fn new(
-        py: Python<'_>,
         calibrations: Vec<PyCalibration>,
         measure_calibrations: Vec<PyMeasureCalibrationDefinition>,
     ) -> PyResult<Self> {
-        Ok(Self(CalibrationSet {
-            calibrations: Vec::<_>::py_try_from(py, &calibrations)?,
-            measure_calibrations: Vec::<_>::py_try_from(py, &measure_calibrations)?,
+        Ok(Self(Calibrations {
+            calibrations: calibrations
+                .into_iter()
+                .map(|c| c.into_inner())
+                .collect::<Vec<Calibration>>()
+                .into(),
+            measure_calibrations: measure_calibrations
+                .into_iter()
+                .map(|c| c.into_inner())
+                .collect::<Vec<MeasureCalibrationDefinition>>()
+                .into(),
         }))
     }
 
     #[getter]
     pub fn calibrations(&self, py: Python<'_>) -> PyResult<Vec<PyCalibration>> {
         self.as_inner().calibrations().to_python(py)
     }
@@ -94,34 +101,42 @@
         self.as_inner().len()
     }
 
     pub fn is_empty(&self) -> bool {
         self.as_inner().is_empty()
     }
 
-    pub fn push_calibration(&mut self, py: Python<'_>, calibration: PyCalibration) -> PyResult<()> {
-        self.as_inner_mut()
-            .push_calibration(Calibration::py_try_from(py, &calibration)?);
-        Ok(())
+    pub fn insert_calibration(
+        &mut self,
+        py: Python<'_>,
+        calibration: PyCalibration,
+    ) -> PyResult<Option<PyCalibration>> {
+        Ok(self
+            .as_inner_mut()
+            .insert_calibration(Calibration::py_try_from(py, &calibration)?)
+            .map(PyCalibration::from))
     }
 
-    pub fn push_measurement_calibration(
+    pub fn insert_measurement_calibration(
         &mut self,
         py: Python<'_>,
         calibration: PyMeasureCalibrationDefinition,
-    ) -> PyResult<()> {
-        self.as_inner_mut().push_measurement_calibration(
-            MeasureCalibrationDefinition::py_try_from(py, &calibration)?,
-        );
-        Ok(())
+    ) -> PyResult<Option<PyMeasureCalibrationDefinition>> {
+        Ok(self
+            .as_inner_mut()
+            .insert_measurement_calibration(MeasureCalibrationDefinition::py_try_from(
+                py,
+                &calibration,
+            )?)
+            .map(PyMeasureCalibrationDefinition::from))
     }
 
     pub fn extend(&mut self, py: Python<'_>, other: PyCalibrationSet) -> PyResult<()> {
         self.as_inner_mut()
-            .extend(CalibrationSet::py_try_from(py, &other)?);
+            .extend(Calibrations::py_try_from(py, &other)?);
         Ok(())
     }
 
     pub fn to_instructions(&self, py: Python<'_>) -> PyResult<Vec<PyInstruction>> {
         self.as_inner().to_instructions().to_python(py)
     }
 }
```

### Comparing `quil-0.7.1rc0/quil-py/src/program/frame.rs` & `quil-0.8.0/quil-py/src/program/frame.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/program/memory.rs` & `quil-0.8.0/quil-py/src/program/memory.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/program/mod.rs` & `quil-0.8.0/quil-py/src/program/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 };
 
 use numpy::{PyArray2, ToPyArray};
 use quil_rs::{
     instruction::{Instruction, QubitPlaceholder, TargetPlaceholder, Waveform},
     program::{
         analysis::{ControlFlowGraph, ControlFlowGraphOwned},
-        CalibrationSet, FrameSet, MemoryRegion,
+        Calibrations, FrameSet, MemoryRegion,
     },
     Program,
 };
 use rigetti_pyo3::{
     create_init_submodule, impl_as_mut_for_wrapper, impl_from_str, impl_parse, impl_repr,
     num_complex::Complex64,
     py_wrap_error, py_wrap_type,
@@ -105,15 +105,15 @@
     #[setter]
     pub fn set_calibrations(
         &mut self,
         py: Python<'_>,
         calibrations: PyCalibrationSet,
     ) -> PyResult<()> {
         let program = self.as_inner_mut();
-        program.calibrations = CalibrationSet::py_try_from(py, &calibrations)?;
+        program.calibrations = Calibrations::py_try_from(py, &calibrations)?;
         Ok(())
     }
 
     #[getter]
     pub fn waveforms(&self, py: Python<'_>) -> PyResult<BTreeMap<String, PyWaveform>> {
         self.as_inner().waveforms.to_python(py)
     }
```

### Comparing `quil-0.7.1rc0/quil-py/src/program/scheduling.rs` & `quil-0.8.0/quil-py/src/program/scheduling.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/src/validation/identifier.rs` & `quil-0.8.0/quil-py/src/validation/identifier.rs`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/test/instructions/test_copy.py` & `quil-0.8.0/quil-py/test/instructions/test_copy.py`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/test/program/test_program.py` & `quil-0.8.0/quil-py/test/program/test_program.py`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil-py/test/test_eq.py` & `quil-0.8.0/quil-py/test/test_eq.py`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/Cargo.lock` & `quil-0.8.0/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstream"
-version = "0.3.2"
+version = "0.6.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
- "is-terminal",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -54,23 +53,29 @@
 checksum = "5ca11d4be1bab0c8bc8734a9aa7bf4ee8316d462a08c6ac5052f888fef5b494b"
 dependencies = [
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anstyle-wincon"
-version = "1.0.1"
+version = "3.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
+checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
 dependencies = [
  "anstyle",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "anyhow"
+version = "1.0.81"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+
+[[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-complex",
  "num-traits",
@@ -173,52 +178,51 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.19"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fd304a20bff958a57f04c4e96a2e7594cc4490a0e809cbd48bb6437edaa452d"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
- "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.19"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01c6a3f08f1fe5662a35cfe393aec09c4df95f60ee93b7556505260f75eee9e1"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.12"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54a9bb5758fc5dfe728d1019941681eccaf0cf8a4189b692a0ee2f2ecf90a050"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
- "heck",
+ "heck 0.5.0",
  "proc-macro2 1.0.78",
  "quote 1.0.35",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.5.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
@@ -509,46 +513,51 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
 
 [[package]]
 name = "indexmap"
-version = "2.2.2"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "824b2ae422412366ba479e8111fd301f7b5faece8149317bb81925979a53f520"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
 
 [[package]]
 name = "insta"
-version = "1.31.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0770b0a3d4c70567f0d58331f3088b0e4c4f56c9b8d764efe654b4a5d46de3a"
+checksum = "1718b3f2b85bb5054baf8ce406e36401f27c3169205f4175504c4b1d98252d3f"
 dependencies = [
  "console",
  "lazy_static",
  "linked-hash-map",
  "similar",
- "yaml-rust",
 ]
 
 [[package]]
 name = "inventory"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a53088c87cf71c9d4f3372a2cb9eea1e7b8a0b1bf8b7f7d23fe5b76dbb07e63b"
@@ -924,14 +933,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
@@ -980,97 +995,110 @@
  "proc-macro2 0.4.30",
  "quote 0.6.13",
  "syn 0.15.44",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
+ "indexmap",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
  "num-complex",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a96fe70b176a89cff78f2fa7b3c930081e163d5379b4dcdf993e3ae29ca662e5"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dac53072f717aa1bfa4db832b39de8c875b7c7af4f4a6fe93cdbf9264cf8383b"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2 1.0.78",
  "pyo3-macros-backend",
  "quote 1.0.35",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7774b5a8282bd4f25f803b1f0d945120be959a36c72e08e7cd031c792fdfd424"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2 1.0.78",
+ "pyo3-build-config",
  "quote 1.0.35",
  "syn 2.0.48",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
+name = "quil-cli"
+version = "0.1.0"
+dependencies = [
+ "anyhow",
+ "clap",
+ "quil-rs",
+]
+
+[[package]]
 name = "quil-py"
-version = "0.7.1-rc.0"
+version = "0.8.0"
 dependencies = [
+ "indexmap",
  "ndarray",
  "numpy",
  "pyo3",
  "pyo3-build-config",
  "quil-rs",
  "rigetti-pyo3",
  "strum",
 ]
 
 [[package]]
 name = "quil-rs"
-version = "0.23.0"
+version = "0.24.0"
 dependencies = [
  "approx",
  "clap",
  "criterion",
  "dot-writer",
  "indexmap",
  "insta",
@@ -1398,17 +1426,17 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "strsim"
-version = "0.10.0"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
 
 [[package]]
 name = "strum"
 version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "723b93e8addf9aa965ebe2d11da6d7540fa2283fcea14b3371ff055f7ba13f5f"
 dependencies = [
@@ -1417,15 +1445,15 @@
 
 [[package]]
 name = "strum_macros"
 version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a3417fc93d76740d974a01654a09777cb500428cc874ca9f45edfe0c4d4cd18"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2 1.0.78",
  "quote 1.0.35",
  "rustversion",
  "syn 2.0.48",
 ]
 
 [[package]]
@@ -1681,14 +1709,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
  "windows-targets 0.48.1",
 ]
 
 [[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.4",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
  "windows_aarch64_gnullvm 0.42.2",
  "windows_aarch64_msvc 0.42.2",
@@ -1711,98 +1748,146 @@
  "windows_i686_msvc 0.48.0",
  "windows_x86_64_gnu 0.48.0",
  "windows_x86_64_gnullvm 0.48.0",
  "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
+name = "windows-targets"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
+]
+
+[[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
-name = "yaml-rust"
-version = "0.4.5"
+name = "windows_x86_64_msvc"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
-dependencies = [
- "linked-hash-map",
-]
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
```

### Comparing `quil-0.7.1rc0/pyproject.toml` & `quil-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
   "Operating System :: OS Independent",
 ]
 
 # PEP 621 specifies the [project] table as the source for project metadata. However, Poetry only supports [tool.poetry]
 # We can remove this table once this issue is resolved: https://github.com/python-poetry/poetry/issues/3332
 [tool.poetry]
 name = "quil"
-version = "0.7.1-rc.0"
+version = "0.8.0"
 description = "A Python package for building and parsing Quil programs."
 readme = "README-py.md"
 authors = ["Rigetti Computing <softapps@rigetti.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.21"
```

### Comparing `quil-0.7.1rc0/quil/expression/__init__.pyi` & `quil-0.8.0/quil/expression/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil/instructions/__init__.pyi` & `quil-0.8.0/quil/instructions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/quil/program/__init__.pyi` & `quil-0.8.0/quil/program/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -318,22 +318,28 @@
         5. All fixed qubits in the calibration definition match those in the gate
         6. All specified parameters in the calibration definition match those in the gate
         """
     def __len__(self) -> int: ...
     def is_empty(self) -> bool:
         """Returns ``True`` if the ``CalibrationSet`` contains no data."""
         ...
-    def push_calibration(self, calibration: Calibration):
+    def insert_calibration(self, calibration: Calibration) -> Optional[Calibration]:
         """
-        Add another gate ``Calibration`` (`DEFCAL`) to the set.
+        Insert another ``Calibration`` (`DEFCAL`) to the set.
+
+        If a calibration with the same name already exists, it is overwritten and this
+        function returns the previous calibration. Otherwise, None is returned.
         """
         ...
-    def push_measurement_calibration(self, calibration: MeasureCalibrationDefinition):
+    def insert_measurement_calibration(self, calibration: MeasureCalibrationDefinition) -> Optional[MeasureCalibrationDefinition]:
         """
         Add another ``MeasureCalibrationDefinition`` (`DEFCAL MEASURE`) to the set
+
+        If a calibration with the same name already exists, it is overwritten and this
+        function returns the previous calibration. Otherwise, None is returned.
         """
     def extend(self, other: CalibrationSet):
         """
         Append another [`CalibrationSet`] onto this one
         """
         ...
     def to_instructions(self):
```

### Comparing `quil-0.7.1rc0/README-py.md` & `quil-0.8.0/README-py.md`

 * *Files identical despite different names*

### Comparing `quil-0.7.1rc0/PKG-INFO` & `quil-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: quil
-Version: 0.7.1rc0
+Version: 0.8.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Summary: A Python package for building and parsing Quil programs.
```

