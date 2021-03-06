include(BCMTest)

find_package(boost_assert)
find_package(boost_array)
find_package(boost_lambda)

bcm_test_link_libraries(boost_fusion
boost::assert
boost::array
boost::lambda
)

##==============================================================================
#    Copyright (c) 2003-2006 Joel de Guzman
#    Copyright (c) 2013 Mateusz Loskot
#
#   Use, modification and distribution is subject to the Boost Software
#   License, Version 1.0. (See accompanying file LICENSE_1_0.txt or copy at
#   http://www.boost.org/LICENSE_1_0.txt)
#==============================================================================
# bring in rules for testing



bcm_test(NAME algorithm_all SOURCES algorithm/all.cpp)
bcm_test(NAME algorithm_any SOURCES algorithm/any.cpp)
bcm_test(NAME algorithm_clear SOURCES algorithm/clear.cpp)
bcm_test(NAME algorithm_copy SOURCES algorithm/copy.cpp)
bcm_test(NAME algorithm_count SOURCES algorithm/count.cpp)
bcm_test(NAME algorithm_count_if SOURCES algorithm/count_if.cpp)
bcm_test(NAME algorithm_erase SOURCES algorithm/erase.cpp)
bcm_test(NAME algorithm_erase_key SOURCES algorithm/erase_key.cpp)
bcm_test(NAME algorithm_filter SOURCES algorithm/filter.cpp)
bcm_test(NAME algorithm_filter_if SOURCES algorithm/filter_if.cpp)
bcm_test(NAME algorithm_find SOURCES algorithm/find.cpp)
bcm_test(NAME algorithm_find_if SOURCES algorithm/find_if.cpp)
bcm_test(NAME algorithm_fold SOURCES algorithm/fold.cpp)
bcm_test(NAME algorithm_for_each SOURCES algorithm/for_each.cpp)
bcm_test(NAME algorithm_insert SOURCES algorithm/insert.cpp)
bcm_test(NAME algorithm_insert_range SOURCES algorithm/insert_range.cpp)
bcm_test(NAME algorithm_iter_fold SOURCES algorithm/iter_fold.cpp)
bcm_test(NAME algorithm_move SOURCES algorithm/move.cpp)
bcm_test(NAME algorithm_none SOURCES algorithm/none.cpp)
bcm_test(NAME algorithm_pop_back SOURCES algorithm/pop_back.cpp)
bcm_test(NAME algorithm_pop_front SOURCES algorithm/pop_front.cpp)
bcm_test(NAME algorithm_push_back SOURCES algorithm/push_back.cpp)
bcm_test(NAME algorithm_push_front SOURCES algorithm/push_front.cpp)
bcm_test(NAME algorithm_remove SOURCES algorithm/remove.cpp)
bcm_test(NAME algorithm_remove_if SOURCES algorithm/remove_if.cpp)
bcm_test(NAME algorithm_replace SOURCES algorithm/replace.cpp)
bcm_test(NAME algorithm_replace_if SOURCES algorithm/replace_if.cpp)
bcm_test(NAME algorithm_reverse_fold SOURCES algorithm/reverse_fold.cpp)
bcm_test(NAME algorithm_reverse_iter_fold SOURCES algorithm/reverse_iter_fold.cpp)
bcm_test(NAME algorithm_reverse SOURCES algorithm/reverse.cpp)
bcm_test(NAME algorithm_segmented_for_each SOURCES algorithm/segmented_for_each.cpp)
bcm_test(NAME algorithm_segmented_find SOURCES algorithm/segmented_find.cpp)
bcm_test(NAME algorithm_segmented_find_if SOURCES algorithm/segmented_find_if.cpp)
bcm_test(NAME algorithm_segmented_fold SOURCES algorithm/segmented_fold.cpp)
bcm_test(NAME algorithm_transform SOURCES algorithm/transform.cpp)
bcm_test(NAME algorithm_join SOURCES algorithm/join.cpp)
bcm_test(NAME algorithm_zip SOURCES algorithm/zip.cpp)
bcm_test(NAME algorithm_zip2 SOURCES algorithm/zip2.cpp)
bcm_test(NAME algorithm_zip_ignore SOURCES algorithm/zip_ignore.cpp)
bcm_test(NAME algorithm_flatten SOURCES algorithm/flatten.cpp)

bcm_test(NAME sequence_as_deque SOURCES sequence/as_deque.cpp)
bcm_test(NAME sequence_as_list SOURCES sequence/as_list.cpp)
bcm_test(NAME sequence_as_map SOURCES sequence/as_map.cpp)
bcm_test(NAME sequence_as_map_assoc SOURCES sequence/as_map_assoc.cpp)
bcm_test(NAME sequence_as_set SOURCES sequence/as_set.cpp)
bcm_test(NAME sequence_as_vector SOURCES sequence/as_vector.cpp)
bcm_test(NAME sequence_boost_tuple SOURCES sequence/boost_tuple.cpp)
bcm_test(NAME sequence_boost_tuple_iterator SOURCES sequence/boost_tuple_iterator.cpp)
bcm_test(NAME sequence_cons SOURCES sequence/cons.cpp)
bcm_test(NAME sequence_convert_boost_tuple SOURCES sequence/convert_boost_tuple.cpp)
bcm_test(NAME sequence_convert_deque SOURCES sequence/convert_deque.cpp)
bcm_test(NAME sequence_convert_list SOURCES sequence/convert_list.cpp)
bcm_test(NAME sequence_convert_std_pair SOURCES sequence/convert_std_pair.cpp)
bcm_test(NAME sequence_convert_std_tuple SOURCES sequence/convert_std_tuple.cpp)
bcm_test(NAME sequence_convert_vector SOURCES sequence/convert_vector.cpp)
bcm_test(NAME sequence_filter_view SOURCES sequence/filter_view.cpp)
bcm_test(NAME sequence_hash SOURCES sequence/hash.cpp)
bcm_test(NAME sequence_io SOURCES sequence/io.cpp)
bcm_test(NAME sequence_iterator_range SOURCES sequence/iterator_range.cpp)
bcm_test(NAME sequence_joint_view SOURCES sequence/joint_view.cpp)
bcm_test(NAME sequence_list_comparison SOURCES sequence/list_comparison.cpp)
bcm_test(NAME sequence_list_construction SOURCES sequence/list_construction.cpp)
bcm_test(NAME sequence_list_copy SOURCES sequence/list_copy.cpp)
bcm_test(NAME sequence_list_iterator SOURCES sequence/list_iterator.cpp)
bcm_test(NAME sequence_list_hash SOURCES sequence/list_hash.cpp)
bcm_test(NAME sequence_list_make SOURCES sequence/list_make.cpp)
bcm_test(NAME sequence_list_misc SOURCES sequence/list_misc.cpp)
bcm_test(NAME sequence_list_mutate SOURCES sequence/list_mutate.cpp)
bcm_test(NAME sequence_list_nest SOURCES sequence/list_nest.cpp)
bcm_test(NAME sequence_list_tie SOURCES sequence/list_tie.cpp)
bcm_test(NAME sequence_list_value_at SOURCES sequence/list_value_at.cpp)
bcm_test(NAME sequence_deque_comparison SOURCES sequence/deque_comparison.cpp)
bcm_test(NAME sequence_deque_construction SOURCES sequence/deque_construction.cpp)
bcm_test(NAME sequence_deque_copy SOURCES sequence/deque_copy.cpp)
bcm_test(NAME sequence_deque_iterator SOURCES sequence/deque_iterator.cpp)
bcm_test(NAME sequence_deque_hash SOURCES sequence/deque_hash.cpp)
bcm_test(NAME sequence_deque_is_constructible SOURCES sequence/deque_is_constructible.cpp COMPILE_ONLY)
bcm_test(NAME sequence_deque_make SOURCES sequence/deque_make.cpp)
bcm_test(NAME sequence_deque_misc SOURCES sequence/deque_misc.cpp)
bcm_test(NAME sequence_deque_move SOURCES sequence/deque_move.cpp)
bcm_test(NAME sequence_deque_mutate SOURCES sequence/deque_mutate.cpp)
bcm_test(NAME sequence_deque_nest SOURCES sequence/deque_nest.cpp)
bcm_test(NAME sequence_deque_tie SOURCES sequence/deque_tie.cpp)
bcm_test(NAME sequence_deque_value_at SOURCES sequence/deque_value_at.cpp)
bcm_test(NAME sequence_front_extended_deque SOURCES sequence/front_extended_deque.cpp)
bcm_test(NAME sequence_back_extended_deque SOURCES sequence/back_extended_deque.cpp)
bcm_test(NAME sequence_make_list SOURCES sequence/make_list.cpp)
bcm_test(NAME sequence_make_vector SOURCES sequence/make_vector.cpp)
bcm_test(NAME sequence_map SOURCES sequence/map.cpp)
bcm_test(NAME sequence_map_comparison SOURCES sequence/map_comparison.cpp)
bcm_test(NAME sequence_map_construction SOURCES sequence/map_construction.cpp)
bcm_test(NAME sequence_map_copy SOURCES sequence/map_copy.cpp)
bcm_test(NAME sequence_map_misc SOURCES sequence/map_misc.cpp)
bcm_test(NAME sequence_map_move SOURCES sequence/map_move.cpp)
bcm_test(NAME sequence_map_mutate SOURCES sequence/map_mutate.cpp)
bcm_test(NAME sequence_map_tie SOURCES sequence/map_tie.cpp)
bcm_test(NAME sequence_nil SOURCES sequence/nil.cpp)
bcm_test(NAME sequence_nview SOURCES sequence/nview.cpp)
bcm_test(NAME sequence_reverse_view SOURCES sequence/reverse_view.cpp)
bcm_test(NAME sequence_segmented_iterator_range SOURCES sequence/segmented_iterator_range.cpp)
bcm_test(NAME sequence_set SOURCES sequence/set.cpp)
bcm_test(NAME sequence_single_view SOURCES sequence/single_view.cpp)
bcm_test(NAME sequence_std_pair SOURCES sequence/std_pair.cpp)
bcm_test(NAME sequence_boost_array SOURCES sequence/boost_array.cpp)
bcm_test(NAME sequence_array SOURCES sequence/array.cpp)
bcm_test(NAME sequence_std_array SOURCES sequence/std_array.cpp)
bcm_test(NAME sequence_tuple_comparison SOURCES sequence/tuple_comparison.cpp)
bcm_test(NAME sequence_tuple_construction SOURCES sequence/tuple_construction.cpp)
bcm_test(NAME sequence_tuple_conversion SOURCES sequence/tuple_conversion.cpp)
bcm_test(NAME sequence_tuple_copy SOURCES sequence/tuple_copy.cpp)
bcm_test(NAME sequence_tuple_element SOURCES sequence/tuple_element.cpp)
bcm_test(NAME sequence_tuple_make SOURCES sequence/tuple_make.cpp)
bcm_test(NAME sequence_tuple_misc SOURCES sequence/tuple_misc.cpp)
bcm_test(NAME sequence_tuple_mutate SOURCES sequence/tuple_mutate.cpp)
bcm_test(NAME sequence_tuple_nest SOURCES sequence/tuple_nest.cpp)
bcm_test(NAME sequence_tuple_hash SOURCES sequence/tuple_hash.cpp)
bcm_test(NAME sequence_tuple_tie SOURCES sequence/tuple_tie.cpp)
bcm_test(NAME sequence_tuple_traits_maybe_variadic_tuple SOURCES sequence/tuple_traits.cpp)
bcm_test(NAME sequence_tuple_traits_no_variadic_tuple SOURCES sequence/tuple_traits.cpp)
target_compile_definitions(sequence_tuple_traits_no_variadic_tuple PUBLIC BOOST_FUSION_DISABLE_VARIADIC_VECTOR)
bcm_test(NAME sequence_transform_view SOURCES sequence/transform_view.cpp)
bcm_test(NAME sequence_vector_comparison SOURCES sequence/vector_comparison.cpp)
bcm_test(NAME sequence_vector_construction SOURCES sequence/vector_construction.cpp)
bcm_test(NAME sequence_vector_conversion SOURCES sequence/vector_conversion.cpp)
bcm_test(NAME sequence_vector_copy SOURCES sequence/vector_copy.cpp)
bcm_test(NAME sequence_vector_iterator SOURCES sequence/vector_iterator.cpp)
bcm_test(NAME sequence_vector_make SOURCES sequence/vector_make.cpp)
bcm_test(NAME sequence_vector_misc SOURCES sequence/vector_misc.cpp)
bcm_test(NAME sequence_vector_move SOURCES sequence/vector_move.cpp)
bcm_test(NAME sequence_vector_mutate SOURCES sequence/vector_mutate.cpp)
bcm_test(NAME sequence_vector_n SOURCES sequence/vector_n.cpp)
bcm_test(NAME sequence_vector_nest SOURCES sequence/vector_nest.cpp)
bcm_test(NAME sequence_vector_hash SOURCES sequence/vector_hash.cpp)
bcm_test(NAME sequence_vector_tie SOURCES sequence/vector_tie.cpp)
bcm_test(NAME sequence_vector_traits_maybe_variadic_vector SOURCES sequence/vector_traits.cpp)
bcm_test(NAME sequence_vector_traits_no_variadic_vector SOURCES sequence/vector_traits.cpp)
target_compile_definitions(sequence_vector_traits_no_variadic_vector PUBLIC BOOST_FUSION_DISABLE_VARIADIC_VECTOR)
bcm_test(NAME sequence_vector_value_at SOURCES sequence/vector_value_at.cpp)
bcm_test(NAME sequence_zip_view SOURCES sequence/zip_view.cpp)
bcm_test(NAME sequence_zip_view2 SOURCES sequence/zip_view2.cpp)
bcm_test(NAME sequence_zip_view_ignore SOURCES sequence/zip_view_ignore.cpp)
bcm_test(NAME sequence_repetitive_view SOURCES sequence/repetitive_view.cpp)
bcm_test(NAME sequence_deduce_sequence SOURCES sequence/deduce_sequence.cpp)
bcm_test(NAME sequence_adapt_adt_named SOURCES sequence/adapt_adt_named.cpp)
bcm_test(NAME sequence_adapt_adt_named_empty SOURCES sequence/adapt_adt_named_empty.cpp)
bcm_test(NAME sequence_adapt_adt SOURCES sequence/adapt_adt.cpp)
bcm_test(NAME sequence_adapt_adt_empty SOURCES sequence/adapt_adt_empty.cpp)
bcm_test(NAME sequence_adapt_assoc_adt_named SOURCES sequence/adapt_assoc_adt_named.cpp)
bcm_test(NAME sequence_adapt_assoc_adt_named_empty SOURCES sequence/adapt_assoc_adt_named_empty.cpp)
bcm_test(NAME sequence_adapt_assoc_adt SOURCES sequence/adapt_assoc_adt.cpp)
bcm_test(NAME sequence_adapt_assoc_adt_empty SOURCES sequence/adapt_assoc_adt_empty.cpp)
bcm_test(NAME sequence_adapt_assoc_struct_named SOURCES sequence/adapt_assoc_struct_named.cpp)
bcm_test(NAME sequence_adapt_assoc_struct_named_empty SOURCES sequence/adapt_assoc_struct_named_empty.cpp)
bcm_test(NAME sequence_adapt_assoc_struct SOURCES sequence/adapt_assoc_struct.cpp)
bcm_test(NAME sequence_adapt_assoc_struct_empty SOURCES sequence/adapt_assoc_struct_empty.cpp)
bcm_test(NAME sequence_adapt_assoc_tpl_adt SOURCES sequence/adapt_assoc_tpl_adt.cpp)
bcm_test(NAME sequence_adapt_assoc_tpl_adt_empty SOURCES sequence/adapt_assoc_tpl_adt_empty.cpp)
bcm_test(NAME sequence_adapt_assoc_tpl_struct SOURCES sequence/adapt_assoc_tpl_struct.cpp)
bcm_test(NAME sequence_adapt_assoc_tpl_struct_empty SOURCES sequence/adapt_assoc_tpl_struct_empty.cpp)
bcm_test(NAME sequence_adapt_struct_named SOURCES sequence/adapt_struct_named.cpp)
bcm_test(NAME sequence_adapt_struct_named_empty SOURCES sequence/adapt_struct_named_empty.cpp)
bcm_test(NAME sequence_adapt_struct SOURCES sequence/adapt_struct.cpp)
bcm_test(NAME sequence_adapt_struct_empty SOURCES sequence/adapt_struct_empty.cpp)
bcm_test(NAME sequence_adapt_tpl_adt SOURCES sequence/adapt_tpl_adt.cpp)
bcm_test(NAME sequence_adapt_tpl_adt_empty SOURCES sequence/adapt_tpl_adt_empty.cpp)
bcm_test(NAME sequence_adapt_tpl_struct SOURCES sequence/adapt_tpl_struct.cpp)
bcm_test(NAME sequence_adapt_tpl_struct_empty SOURCES sequence/adapt_tpl_struct_empty.cpp)
bcm_test(NAME sequence_adt_attribute_proxy SOURCES sequence/adt_attribute_proxy.cpp)
bcm_test(NAME sequence_define_struct SOURCES sequence/define_struct.cpp)
bcm_test(NAME sequence_define_struct_empty SOURCES sequence/define_struct_empty.cpp)
bcm_test(NAME sequence_define_struct_move SOURCES sequence/define_struct_move.cpp)
bcm_test(NAME sequence_define_struct_inline SOURCES sequence/define_struct_inline.cpp)
bcm_test(NAME sequence_define_struct_inline_empty SOURCES sequence/define_struct_inline_empty.cpp)
bcm_test(NAME sequence_define_struct_inline_move SOURCES sequence/define_struct_inline_move.cpp)
bcm_test(NAME sequence_define_assoc_struct SOURCES sequence/define_assoc_struct.cpp)
bcm_test(NAME sequence_define_assoc_struct_empty SOURCES sequence/define_assoc_struct_empty.cpp)
bcm_test(NAME sequence_define_assoc_struct_move SOURCES sequence/define_assoc_struct_move.cpp)
bcm_test(NAME sequence_define_tpl_struct SOURCES sequence/define_tpl_struct.cpp)
bcm_test(NAME sequence_define_tpl_struct_empty SOURCES sequence/define_tpl_struct_empty.cpp)
bcm_test(NAME sequence_define_tpl_struct_move SOURCES sequence/define_tpl_struct_move.cpp)
bcm_test(NAME sequence_define_tpl_struct_inline SOURCES sequence/define_tpl_struct_inline.cpp)
bcm_test(NAME sequence_define_tpl_struct_inline_empty SOURCES sequence/define_tpl_struct_inline_empty.cpp)
bcm_test(NAME sequence_define_tpl_struct_inline_move SOURCES sequence/define_tpl_struct_inline_move.cpp)
bcm_test(NAME sequence_define_assoc_tpl_struct SOURCES sequence/define_assoc_tpl_struct.cpp)
bcm_test(NAME sequence_define_assoc_tpl_struct_empty SOURCES sequence/define_assoc_tpl_struct_empty.cpp)
bcm_test(NAME sequence_define_assoc_tpl_struct_move SOURCES sequence/define_assoc_tpl_struct_move.cpp)
bcm_test(NAME sequence_std_tuple SOURCES sequence/std_tuple.cpp)
bcm_test(NAME sequence_std_tuple_iterator SOURCES sequence/std_tuple_iterator.cpp)
bcm_test(NAME sequence_ref_vector SOURCES sequence/ref_vector.cpp)
bcm_test(NAME sequence_flatten_view SOURCES sequence/flatten_view.cpp)

bcm_test(NAME sequence_size SOURCES sequence/size.cpp COMPILE_ONLY)

bcm_test(NAME functional_fused SOURCES functional/fused.cpp)
bcm_test(NAME functional_fused_function_object SOURCES functional/fused_function_object.cpp)
bcm_test(NAME functional_fused_procedure SOURCES functional/fused_procedure.cpp)
bcm_test(NAME functional_unfused SOURCES functional/unfused.cpp)
bcm_test(NAME functional_unfused_typed SOURCES functional/unfused_typed.cpp)
bcm_test(NAME functional_make_fused SOURCES functional/make_fused.cpp)
bcm_test(NAME functional_make_fused_function_object SOURCES functional/make_fused_function_object.cpp)
bcm_test(NAME functional_make_fused_procedure SOURCES functional/make_fused_procedure.cpp)
bcm_test(NAME functional_make_unfused SOURCES functional/make_unfused.cpp)
bcm_test(NAME functional_invoke SOURCES functional/invoke.cpp)
bcm_test(NAME functional_invoke_function_object SOURCES functional/invoke_function_object.cpp)
bcm_test(NAME functional_invoke_procedure SOURCES functional/invoke_procedure.cpp)
bcm_test(NAME sequence_swap SOURCES sequence/swap.cpp)

bcm_test(NAME support_pair_deque SOURCES support/pair_deque.cpp COMPILE_ONLY)
bcm_test(NAME support_pair_list SOURCES support/pair_list.cpp COMPILE_ONLY)
bcm_test(NAME support_pair_map SOURCES support/pair_map.cpp COMPILE_ONLY)
bcm_test(NAME support_pair_set SOURCES support/pair_set.cpp COMPILE_ONLY)
bcm_test(NAME support_pair_vector SOURCES support/pair_vector.cpp COMPILE_ONLY)
bcm_test(NAME support_pair_nest SOURCES support/pair_nest.cpp COMPILE_ONLY)
bcm_test(NAME support_index_sequence SOURCES support/index_sequence.cpp COMPILE_ONLY)
bcm_test(NAME support_and SOURCES support/and.cpp COMPILE_ONLY)

#   [ compile-fail xxx.cpp :  :  :  :  ]


