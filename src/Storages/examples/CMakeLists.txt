add_executable (merge_selector merge_selector.cpp)
target_link_libraries (merge_selector PRIVATE dbms)

add_executable (merge_selector2 merge_selector2.cpp)
target_link_libraries (merge_selector2 PRIVATE dbms)

add_executable (get_current_inserts_in_replicated get_current_inserts_in_replicated.cpp)
target_link_libraries (get_current_inserts_in_replicated PRIVATE dbms clickhouse_common_config clickhouse_common_zookeeper string_utils)

add_executable (get_abandonable_lock_in_all_partitions get_abandonable_lock_in_all_partitions.cpp)
target_link_libraries (get_abandonable_lock_in_all_partitions PRIVATE dbms clickhouse_common_config clickhouse_common_zookeeper)
