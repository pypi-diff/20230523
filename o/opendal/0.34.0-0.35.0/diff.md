# Comparing `tmp/opendal-0.34.0.tar.gz` & `tmp/opendal-0.35.0.tar.gz`

## Comparing `opendal-0.34.0.tar` & `opendal-0.35.0.tar`

### file list

```diff
@@ -1,284 +1,298 @@
--rw-r--r--   0        0        0     6578 1970-01-01 00:00:00.000000 opendal-0.34.0/local_dependencies/opendal/Cargo.toml
--rw-r--r--   0     1001      123    69956 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/CHANGELOG.md
--rw-r--r--   0     1001      123     1114 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/CONTRIBUTING.md
--rw-r--r--   0     1001      123     6804 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/README.md
--rw-r--r--   0     1001      123      378 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/benches/README.md
--rw-r--r--   0     1001      123      672 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/benches/ops/README.md
--rw-r--r--   0     1001      123      979 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/benches/ops/main.rs
--rw-r--r--   0     1001      123     5574 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/benches/ops/read.rs
--rw-r--r--   0     1001      123     2527 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/benches/ops/utils.rs
--rw-r--r--   0     1001      123     2163 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/benches/ops/write.rs
--rw-r--r--   0     1001      123     1823 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/examples/object.rs
--rw-r--r--   0     1001      123     1290 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
--rw-r--r--   0     1001      123     7682 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
--rw-r--r--   0     1001      123     6142 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/concepts.rs
--rw-r--r--   0     1001      123      982 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/features.md
--rw-r--r--   0     1001      123    10879 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/internals/accessor.rs
--rw-r--r--   0     1001      123     1765 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/internals/layer.rs
--rw-r--r--   0     1001      123     3409 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/internals/mod.rs
--rw-r--r--   0     1001      123     1458 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/mod.rs
--rw-r--r--   0     1001      123     3436 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
--rw-r--r--   0     1001      123     5329 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
--rw-r--r--   0     1001      123     4885 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
--rw-r--r--   0     1001      123     5428 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
--rw-r--r--   0     1001      123     3341 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
--rw-r--r--   0     1001      123     4425 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
--rw-r--r--   0     1001      123     2902 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
--rw-r--r--   0     1001      123    12349 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
--rw-r--r--   0     1001      123     2538 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
--rw-r--r--   0     1001      123     2347 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
--rw-r--r--   0     1001      123     2805 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
--rw-r--r--   0     1001      123     1803 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
--rw-r--r--   0     1001      123     4733 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
--rw-r--r--   0     1001      123     2184 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
--rw-r--r--   0     1001      123     5771 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
--rw-r--r--   0     1001      123     8563 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
--rw-r--r--   0     1001      123     3113 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
--rw-r--r--   0     1001      123     4321 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
--rw-r--r--   0     1001      123     1881 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
--rw-r--r--   0     1001      123     2926 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
--rw-r--r--   0     1001      123     2246 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
--rw-r--r--   0     1001      123     6523 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
--rw-r--r--   0     1001      123     4792 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
--rw-r--r--   0     1001      123    10091 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
--rw-r--r--   0     1001      123     2508 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
--rw-r--r--   0     1001      123     2670 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
--rw-r--r--   0     1001      123     8059 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
--rw-r--r--   0     1001      123     2472 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
--rw-r--r--   0     1001      123     4452 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
--rw-r--r--   0     1001      123     2534 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
--rw-r--r--   0     1001      123     3693 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
--rw-r--r--   0     1001      123     3255 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
--rw-r--r--   0     1001      123     4133 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
--rw-r--r--   0     1001      123     4408 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
--rw-r--r--   0     1001      123     4230 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
--rw-r--r--   0     1001      123     3172 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
--rw-r--r--   0     1001      123     2687 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
--rw-r--r--   0     1001      123     4554 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
--rw-r--r--   0     1001      123    24200 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/docs/upgrade.md
--rw-r--r--   0     1001      123     6462 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/chaos.rs
--rw-r--r--   0     1001      123    20699 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/complete.rs
--rw-r--r--   0     1001      123     9110 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
--rw-r--r--   0     1001      123    16005 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/error_context.rs
--rw-r--r--   0     1001      123    13789 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/immutable_index.rs
--rw-r--r--   0     1001      123    49059 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/logging.rs
--rw-r--r--   0     1001      123    13014 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/madsim.rs
--rw-r--r--   0     1001      123    29528 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/metrics.rs
--rw-r--r--   0     1001      123    12210 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/minitrace.rs
--rw-r--r--   0     1001      123     2205 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/mod.rs
--rw-r--r--   0     1001      123    12947 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/oteltrace.rs
--rw-r--r--   0     1001      123    22886 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/prometheus.rs
--rw-r--r--   0     1001      123    35932 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/retry.rs
--rw-r--r--   0     1001      123    11818 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/tracing.rs
--rw-r--r--   0     1001      123     3393 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/layers/type_eraser.rs
--rw-r--r--   0     1001      123     3570 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/lib.rs
--rw-r--r--   0     1001      123    18011 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/accessor.rs
--rw-r--r--   0     1001      123     5049 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
--rw-r--r--   0     1001      123    10358 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
--rw-r--r--   0     1001      123     1020 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
--rw-r--r--   0     1001      123     1566 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/mod.rs
--rw-r--r--   0     1001      123     5400 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
--rw-r--r--   0     1001      123    10344 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
--rw-r--r--   0     1001      123     1067 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
--rw-r--r--   0     1001      123     1934 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/chrono_util.rs
--rw-r--r--   0     1001      123     5973 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/body.rs
--rw-r--r--   0     1001      123    10135 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
--rw-r--r--   0     1001      123    10534 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
--rw-r--r--   0     1001      123     5424 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/client.rs
--rw-r--r--   0     1001      123     3415 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/error.rs
--rw-r--r--   0     1001      123    11165 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/header.rs
--rw-r--r--   0     1001      123     2159 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/mod.rs
--rw-r--r--   0     1001      123    21679 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/multipart.rs
--rw-r--r--   0     1001      123     2962 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/uri.rs
--rw-r--r--   0     1001      123    11222 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/layer.rs
--rw-r--r--   0     1001      123     1950 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/mod.rs
--rw-r--r--   0     1001      123     9434 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/cursor.rs
--rw-r--r--   0     1001      123     2512 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/entry.rs
--rw-r--r--   0     1001      123     3666 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
--rw-r--r--   0     1001      123     1006 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
--rw-r--r--   0     1001      123    15399 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
--rw-r--r--   0     1001      123     4150 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
--rw-r--r--   0     1001      123     1686 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
--rw-r--r--   0     1001      123     4579 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
--rw-r--r--   0     1001      123     2001 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/mod.rs
--rw-r--r--   0     1001      123     3516 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/page.rs
--rw-r--r--   0     1001      123    10680 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/read.rs
--rw-r--r--   0     1001      123     9149 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
--rw-r--r--   0     1001      123     6894 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
--rw-r--r--   0     1001      123     5198 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/oio/write.rs
--rw-r--r--   0     1001      123     4081 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/operation.rs
--rw-r--r--   0     1001      123    11671 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/path.rs
--rw-r--r--   0     1001      123     6307 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/rps.rs
--rw-r--r--   0     1001      123     1396 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/serde_util.rs
--rw-r--r--   0     1001      123     1077 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/raw/version.rs
--rw-r--r--   0     1001      123    29167 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azblob/backend.rs
--rw-r--r--   0     1001      123     5544 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azblob/batch.rs
--rw-r--r--   0     1001      123    11380 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azblob/core.rs
--rw-r--r--   0     1001      123     5870 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azblob/error.rs
--rw-r--r--   0     1001      123      913 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azblob/mod.rs
--rw-r--r--   0     1001      123    14196 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azblob/pager.rs
--rw-r--r--   0     1001      123     2079 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azblob/writer.rs
--rw-r--r--   0     1001      123    16539 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/backend.rs
--rw-r--r--   0     1001      123     9557 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/core.rs
--rw-r--r--   0     1001      123     3519 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/error.rs
--rw-r--r--   0     1001      123      900 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/mod.rs
--rw-r--r--   0     1001      123     5647 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/pager.rs
--rw-r--r--   0     1001      123     2736 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/writer.rs
--rw-r--r--   0     1001      123     4186 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/dashmap/backend.rs
--rw-r--r--   0     1001      123      859 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/dashmap/mod.rs
--rw-r--r--   0     1001      123    23569 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/fs/backend.rs
--rw-r--r--   0     1001      123     1424 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/fs/error.rs
--rw-r--r--   0     1001      123      884 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/fs/mod.rs
--rw-r--r--   0     1001      123     4430 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/fs/pager.rs
--rw-r--r--   0     1001      123     3092 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/fs/writer.rs
--rw-r--r--   0     1001      123    16897 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ftp/backend.rs
--rw-r--r--   0     1001      123     1808 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ftp/err.rs
--rw-r--r--   0     1001      123      894 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ftp/mod.rs
--rw-r--r--   0     1001      123     2504 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ftp/pager.rs
--rw-r--r--   0     1001      123     4208 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ftp/util.rs
--rw-r--r--   0     1001      123     1900 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ftp/writer.rs
--rw-r--r--   0     1001      123    21315 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gcs/backend.rs
--rw-r--r--   0     1001      123    16245 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gcs/core.rs
--rw-r--r--   0     1001      123     3512 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gcs/error.rs
--rw-r--r--   0     1001      123      905 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gcs/mod.rs
--rw-r--r--   0     1001      123    10592 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gcs/pager.rs
--rw-r--r--   0     1001      123     2820 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gcs/uri.rs
--rw-r--r--   0     1001      123     6340 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gcs/writer.rs
--rw-r--r--   0     1001      123     8028 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/backend.rs
--rw-r--r--   0     1001      123     4250 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/builder.rs
--rw-r--r--   0     1001      123     1743 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/error.rs
--rw-r--r--   0     1001      123      894 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/mod.rs
--rw-r--r--   0     1001      123     1975 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/writer.rs
--rw-r--r--   0     1001      123    20863 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ghac/backend.rs
--rw-r--r--   0     1001      123     1908 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ghac/error.rs
--rw-r--r--   0     1001      123      877 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ghac/mod.rs
--rw-r--r--   0     1001      123     2375 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ghac/writer.rs
--rw-r--r--   0     1001      123    16085 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/backend.rs
--rw-r--r--   0     1001      123     1497 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/error.rs
--rw-r--r--   0     1001      123      888 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/mod.rs
--rw-r--r--   0     1001      123     3315 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/pager.rs
--rw-r--r--   0     1001      123     2461 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/writer.rs
--rw-r--r--   0     1001      123    16363 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/http/backend.rs
--rw-r--r--   0     1001      123     1875 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/http/error.rs
--rw-r--r--   0     1001      123      265 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
--rw-r--r--   0     1001      123      865 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/http/mod.rs
--rw-r--r--   0     1001      123    17080 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/backend.rs
--rw-r--r--   0     1001      123     1871 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/error.rs
--rw-r--r--   0     1001      123     8200 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
--rw-r--r--   0     1001      123      875 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/mod.rs
--rw-r--r--   0     1001      123     9252 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
--rw-r--r--   0     1001      123     3946 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
--rw-r--r--   0     1001      123     2790 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/error.rs
--rw-r--r--   0     1001      123      903 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
--rw-r--r--   0     1001      123     3819 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
--rw-r--r--   0     1001      123     1753 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
--rw-r--r--   0     1001      123     5712 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/memcached/ascii.rs
--rw-r--r--   0     1001      123     9250 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/memcached/backend.rs
--rw-r--r--   0     1001      123      875 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/memcached/mod.rs
--rw-r--r--   0     1001      123     4434 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/memory/backend.rs
--rw-r--r--   0     1001      123      857 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/memory/mod.rs
--rw-r--r--   0     1001      123     4064 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/mod.rs
--rw-r--r--   0     1001      123     8174 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/moka/backend.rs
--rw-r--r--   0     1001      123      853 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/moka/mod.rs
--rw-r--r--   0     1001      123    13967 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/obs/backend.rs
--rw-r--r--   0     1001      123     7436 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/obs/core.rs
--rw-r--r--   0     1001      123     3492 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/obs/error.rs
--rw-r--r--   0     1001      123      896 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/obs/mod.rs
--rw-r--r--   0     1001      123     6027 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/obs/pager.rs
--rw-r--r--   0     1001      123     2057 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/obs/writer.rs
--rw-r--r--   0     1001      123     6524 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/backend.rs
--rw-r--r--   0     1001      123     4373 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/builder.rs
--rw-r--r--   0     1001      123     1743 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/error.rs
--rw-r--r--   0     1001      123      898 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/mod.rs
--rw-r--r--   0     1001      123     2189 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/writer.rs
--rw-r--r--   0     1001      123    22936 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/oss/backend.rs
--rw-r--r--   0     1001      123    24223 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/oss/core.rs
--rw-r--r--   0     1001      123     3407 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/oss/error.rs
--rw-r--r--   0     1001      123      896 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/oss/mod.rs
--rw-r--r--   0     1001      123     7006 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/oss/pager.rs
--rw-r--r--   0     1001      123     6676 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/oss/writer.rs
--rw-r--r--   0     1001      123    10832 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/redis/backend.rs
--rw-r--r--   0     1001      123      855 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/redis/mod.rs
--rw-r--r--   0     1001      123     5749 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
--rw-r--r--   0     1001      123      859 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
--rw-r--r--   0     1001      123    41967 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/s3/backend.rs
--rw-r--r--   0     1001      123     3395 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/s3/compatible_services.md
--rw-r--r--   0     1001      123    28632 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/s3/core.rs
--rw-r--r--   0     1001      123     4749 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/s3/error.rs
--rw-r--r--   0     1001      123      894 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/s3/mod.rs
--rw-r--r--   0     1001      123     7387 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/s3/pager.rs
--rw-r--r--   0     1001      123     7259 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/s3/writer.rs
--rw-r--r--   0     1001      123    14662 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sftp/backend.rs
--rw-r--r--   0     1001      123     2894 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sftp/error.rs
--rw-r--r--   0     1001      123      899 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sftp/mod.rs
--rw-r--r--   0     1001      123     2700 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sftp/pager.rs
--rw-r--r--   0     1001      123     3384 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sftp/utils.rs
--rw-r--r--   0     1001      123     1677 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sftp/writer.rs
--rw-r--r--   0     1001      123     5713 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sled/backend.rs
--rw-r--r--   0     1001      123      854 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/sled/mod.rs
--rw-r--r--   0     1001      123     9774 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/supabase/backend.rs
--rw-r--r--   0     1001      123     8021 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/supabase/core.rs
--rw-r--r--   0     1001      123     2582 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/supabase/error.rs
--rw-r--r--   0     1001      123      894 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/supabase/mod.rs
--rw-r--r--   0     1001      123     2382 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/supabase/writer.rs
--rw-r--r--   0     1001      123     4724 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
--rw-r--r--   0     1001      123     3636 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
--rw-r--r--   0     1001      123     1743 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
--rw-r--r--   0     1001      123      912 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
--rw-r--r--   0     1001      123     2055 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
--rw-r--r--   0     1001      123    39155 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/backend.rs
--rw-r--r--   0     1001      123    29726 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/core.rs
--rw-r--r--   0     1001      123     3711 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/error.rs
--rw-r--r--   0     1001      123      902 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/mod.rs
--rw-r--r--   0     1001      123     7061 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/pager.rs
--rw-r--r--   0     1001      123     2666 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/writer.rs
--rw-r--r--   0     1001      123    20963 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/backend.rs
--rw-r--r--   0     1001      123     1743 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/error.rs
--rw-r--r--   0     1001      123      130 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
--rw-r--r--   0     1001      123      626 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
--rw-r--r--   0     1001      123      531 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
--rw-r--r--   0     1001      123    16965 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/list_response.rs
--rw-r--r--   0     1001      123      911 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/mod.rs
--rw-r--r--   0     1001      123     2560 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/pager.rs
--rw-r--r--   0     1001      123     2066 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webdav/writer.rs
--rw-r--r--   0     1001      123    19851 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
--rw-r--r--   0     1001      123     4085 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/error.rs
--rw-r--r--   0     1001      123     4679 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/message.rs
--rw-r--r--   0     1001      123      907 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
--rw-r--r--   0     1001      123     2452 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
--rw-r--r--   0     1001      123     2076 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
--rw-r--r--   0     1001      123     3368 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/builder.rs
--rw-r--r--   0     1001      123     6340 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/capability.rs
--rw-r--r--   0     1001      123     2494 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/entry.rs
--rw-r--r--   0     1001      123    12002 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/error.rs
--rw-r--r--   0     1001      123     7417 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/list.rs
--rw-r--r--   0     1001      123    16557 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/metadata.rs
--rw-r--r--   0     1001      123     1511 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/mod.rs
--rw-r--r--   0     1001      123     1747 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/mode.rs
--rw-r--r--   0     1001      123    24284 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
--rw-r--r--   0     1001      123     8731 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/operator/builder.rs
--rw-r--r--   0     1001      123     2921 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/operator/metadata.rs
--rw-r--r--   0     1001      123     1098 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/operator/mod.rs
--rw-r--r--   0     1001      123    44001 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/operator/operator.rs
--rw-r--r--   0     1001      123    10775 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/ops.rs
--rw-r--r--   0     1001      123     9571 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/reader.rs
--rw-r--r--   0     1001      123     6584 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/scheme.rs
--rw-r--r--   0     1001      123    10795 2023-05-09 08:40:34.000000 opendal-0.34.0/local_dependencies/opendal/src/types/writer.rs
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 opendal-0.34.0/Cargo.toml
--rw-r--r--   0     1001      123      709 2023-05-09 08:40:34.000000 opendal-0.34.0/.gitignore
--rw-r--r--   0     1001      123     2212 2023-05-09 08:40:34.000000 opendal-0.34.0/CONTRIBUTING.md
--rw-r--r--   0     1001      123      982 2023-05-09 08:40:34.000000 opendal-0.34.0/README.md
--rw-r--r--   0     1001      123      765 2023-05-09 08:40:34.000000 opendal-0.34.0/benchmark/README.md
--rw-r--r--   0     1001      123     2426 2023-05-09 08:40:34.000000 opendal-0.34.0/benchmark/async_opendal_benchmark.py
--rw-r--r--   0     1001      123     2955 2023-05-09 08:40:34.000000 opendal-0.34.0/benchmark/async_origin_s3_benchmark_with_gevent.py
--rw-r--r--   0     1001      123      917 2023-05-09 08:40:34.000000 opendal-0.34.0/examples/object.ipynb
--rw-r--r--   0     1001      123     1665 2023-05-09 08:40:34.000000 opendal-0.34.0/pyproject.toml
--rw-r--r--   0     1001      123      866 2023-05-09 08:40:34.000000 opendal-0.34.0/python/opendal/__init__.py
--rw-r--r--   0     1001      123     2917 2023-05-09 08:40:34.000000 opendal-0.34.0/python/opendal/__init__.pyi
--rw-r--r--   0     1001      123    11963 2023-05-09 08:40:34.000000 opendal-0.34.0/src/asyncio.rs
--rw-r--r--   0     1001      123     3311 2023-05-09 08:40:34.000000 opendal-0.34.0/src/layers.rs
--rw-r--r--   0     1001      123    13929 2023-05-09 08:40:34.000000 opendal-0.34.0/src/lib.rs
--rw-r--r--   0     1001      123     1604 2023-05-09 08:40:34.000000 opendal-0.34.0/tests/binding.feature
--rw-r--r--   0     1001      123     2942 2023-05-09 08:40:34.000000 opendal-0.34.0/tests/steps/binding.py
--rw-r--r--   0     1001      123   131926 2023-05-09 08:40:34.000000 opendal-0.34.0/Cargo.lock
--rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 opendal-0.34.0/PKG-INFO
+-rw-r--r--   0        0        0     6232 1970-01-01 00:00:00.000000 opendal-0.35.0/local_dependencies/opendal/Cargo.toml
+-rw-r--r--   0     1001      123    72241 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/CHANGELOG.md
+-rw-r--r--   0     1001      123     1114 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/CONTRIBUTING.md
+-rw-r--r--   0     1001      123     6804 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/README.md
+-rw-r--r--   0     1001      123      378 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/README.md
+-rw-r--r--   0     1001      123      672 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/README.md
+-rw-r--r--   0     1001      123      979 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/main.rs
+-rw-r--r--   0     1001      123     5574 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/read.rs
+-rw-r--r--   0     1001      123     2792 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/utils.rs
+-rw-r--r--   0     1001      123     2163 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/benches/ops/write.rs
+-rw-r--r--   0     1001      123     1823 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/examples/object.rs
+-rw-r--r--   0     1001      123     1290 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/mod.rs
+-rw-r--r--   0     1001      123     7682 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md
+-rw-r--r--   0     1001      123     6142 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/concepts.rs
+-rw-r--r--   0     1001      123      982 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/features.md
+-rw-r--r--   0     1001      123    10879 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/internals/accessor.rs
+-rw-r--r--   0     1001      123     1765 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/internals/layer.rs
+-rw-r--r--   0     1001      123     3409 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/internals/mod.rs
+-rw-r--r--   0     1001      123     1458 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3436 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md
+-rw-r--r--   0     1001      123     5329 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md
+-rw-r--r--   0     1001      123     4885 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md
+-rw-r--r--   0     1001      123     5428 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md
+-rw-r--r--   0     1001      123     3341 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md
+-rw-r--r--   0     1001      123     4425 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md
+-rw-r--r--   0     1001      123     2902 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md
+-rw-r--r--   0     1001      123    12349 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md
+-rw-r--r--   0     1001      123     2538 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md
+-rw-r--r--   0     1001      123     2347 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md
+-rw-r--r--   0     1001      123     2805 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md
+-rw-r--r--   0     1001      123     1803 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md
+-rw-r--r--   0     1001      123     4733 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md
+-rw-r--r--   0     1001      123     2184 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md
+-rw-r--r--   0     1001      123     5771 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md
+-rw-r--r--   0     1001      123     8563 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md
+-rw-r--r--   0     1001      123     3113 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md
+-rw-r--r--   0     1001      123     4321 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md
+-rw-r--r--   0     1001      123     1881 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md
+-rw-r--r--   0     1001      123     2926 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md
+-rw-r--r--   0     1001      123     2246 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md
+-rw-r--r--   0     1001      123     6523 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md
+-rw-r--r--   0     1001      123     4792 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md
+-rw-r--r--   0     1001      123    10091 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md
+-rw-r--r--   0     1001      123     2508 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md
+-rw-r--r--   0     1001      123     2670 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md
+-rw-r--r--   0     1001      123     8059 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md
+-rw-r--r--   0     1001      123     2472 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md
+-rw-r--r--   0     1001      123     4452 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md
+-rw-r--r--   0     1001      123     2534 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md
+-rw-r--r--   0     1001      123     3693 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md
+-rw-r--r--   0     1001      123     3255 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md
+-rw-r--r--   0     1001      123     4133 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md
+-rw-r--r--   0     1001      123     4408 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md
+-rw-r--r--   0     1001      123     4230 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md
+-rw-r--r--   0     1001      123     3172 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md
+-rw-r--r--   0     1001      123     2687 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md
+-rw-r--r--   0     1001      123     4554 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/mod.rs
+-rw-r--r--   0     1001      123    24636 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/docs/upgrade.md
+-rw-r--r--   0     1001      123     6641 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/chaos.rs
+-rw-r--r--   0     1001      123    22169 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/complete.rs
+-rw-r--r--   0     1001      123     9848 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/concurrent_limit.rs
+-rw-r--r--   0     1001      123    17440 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/error_context.rs
+-rw-r--r--   0     1001      123    14233 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/immutable_index.rs
+-rw-r--r--   0     1001      123    52926 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/logging.rs
+-rw-r--r--   0     1001      123    13301 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/madsim.rs
+-rw-r--r--   0     1001      123    29707 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/metrics.rs
+-rw-r--r--   0     1001      123    12389 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/minitrace.rs
+-rw-r--r--   0     1001      123     2205 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/mod.rs
+-rw-r--r--   0     1001      123    13121 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/oteltrace.rs
+-rw-r--r--   0     1001      123    23065 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/prometheus.rs
+-rw-r--r--   0     1001      123    38385 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/retry.rs
+-rw-r--r--   0     1001      123    11997 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/tracing.rs
+-rw-r--r--   0     1001      123     3663 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/layers/type_eraser.rs
+-rw-r--r--   0     1001      123     3570 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/lib.rs
+-rw-r--r--   0     1001      123    18884 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/accessor.rs
+-rw-r--r--   0     1001      123     5049 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs
+-rw-r--r--   0     1001      123    10382 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs
+-rw-r--r--   0     1001      123     1020 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs
+-rw-r--r--   0     1001      123     1566 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/mod.rs
+-rw-r--r--   0     1001      123     5407 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs
+-rw-r--r--   0     1001      123    10368 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs
+-rw-r--r--   0     1001      123     1067 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs
+-rw-r--r--   0     1001      123     1934 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/chrono_util.rs
+-rw-r--r--   0     1001      123     5973 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/body.rs
+-rw-r--r--   0     1001      123    10135 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs
+-rw-r--r--   0     1001      123    10534 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs
+-rw-r--r--   0     1001      123     5424 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/client.rs
+-rw-r--r--   0     1001      123     3415 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/error.rs
+-rw-r--r--   0     1001      123    11165 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/header.rs
+-rw-r--r--   0     1001      123     2159 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/mod.rs
+-rw-r--r--   0     1001      123    21679 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/multipart.rs
+-rw-r--r--   0     1001      123     2962 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/uri.rs
+-rw-r--r--   0     1001      123    11756 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/layer.rs
+-rw-r--r--   0     1001      123     1950 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/mod.rs
+-rw-r--r--   0     1001      123     3018 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/append.rs
+-rw-r--r--   0     1001      123     9434 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/cursor.rs
+-rw-r--r--   0     1001      123     2512 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/entry.rs
+-rw-r--r--   0     1001      123     3666 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1006 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs
+-rw-r--r--   0     1001      123    15427 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs
+-rw-r--r--   0     1001      123     4150 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs
+-rw-r--r--   0     1001      123     1686 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs
+-rw-r--r--   0     1001      123     4579 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs
+-rw-r--r--   0     1001      123     2097 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/mod.rs
+-rw-r--r--   0     1001      123     3516 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/page.rs
+-rw-r--r--   0     1001      123    10670 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/read.rs
+-rw-r--r--   0     1001      123     9177 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs
+-rw-r--r--   0     1001      123     6894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs
+-rw-r--r--   0     1001      123     5206 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/oio/write.rs
+-rw-r--r--   0     1001      123     3953 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/operation.rs
+-rw-r--r--   0     1001      123    11671 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/path.rs
+-rw-r--r--   0     1001      123     6507 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/rps.rs
+-rw-r--r--   0     1001      123     1396 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/serde_util.rs
+-rw-r--r--   0     1001      123     1077 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/raw/version.rs
+-rw-r--r--   0     1001      123    26673 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/backend.rs
+-rw-r--r--   0     1001      123     5544 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/batch.rs
+-rw-r--r--   0     1001      123    11380 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/core.rs
+-rw-r--r--   0     1001      123     2286 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/docs.md
+-rw-r--r--   0     1001      123     5870 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/error.rs
+-rw-r--r--   0     1001      123      913 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/mod.rs
+-rw-r--r--   0     1001      123    14196 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/pager.rs
+-rw-r--r--   0     1001      123     2079 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azblob/writer.rs
+-rw-r--r--   0     1001      123    16596 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/backend.rs
+-rw-r--r--   0     1001      123     9557 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/core.rs
+-rw-r--r--   0     1001      123     3519 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/error.rs
+-rw-r--r--   0     1001      123      900 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/mod.rs
+-rw-r--r--   0     1001      123     5647 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/pager.rs
+-rw-r--r--   0     1001      123     2736 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/writer.rs
+-rw-r--r--   0     1001      123    14710 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/backend.rs
+-rw-r--r--   0     1001      123     8178 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/core.rs
+-rw-r--r--   0     1001      123     3492 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/error.rs
+-rw-r--r--   0     1001      123      896 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/mod.rs
+-rw-r--r--   0     1001      123     5963 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/pager.rs
+-rw-r--r--   0     1001      123     2057 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/cos/writer.rs
+-rw-r--r--   0     1001      123     4186 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/backend.rs
+-rw-r--r--   0     1001      123      859 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/mod.rs
+-rw-r--r--   0     1001      123    23672 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/backend.rs
+-rw-r--r--   0     1001      123     1424 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/error.rs
+-rw-r--r--   0     1001      123      884 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/mod.rs
+-rw-r--r--   0     1001      123     4430 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/pager.rs
+-rw-r--r--   0     1001      123     3092 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/fs/writer.rs
+-rw-r--r--   0     1001      123    16921 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/backend.rs
+-rw-r--r--   0     1001      123     1808 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/err.rs
+-rw-r--r--   0     1001      123      894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/mod.rs
+-rw-r--r--   0     1001      123     2504 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/pager.rs
+-rw-r--r--   0     1001      123     4208 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/util.rs
+-rw-r--r--   0     1001      123     1900 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ftp/writer.rs
+-rw-r--r--   0     1001      123    21339 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/backend.rs
+-rw-r--r--   0     1001      123    16245 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/core.rs
+-rw-r--r--   0     1001      123     3512 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/error.rs
+-rw-r--r--   0     1001      123      905 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/mod.rs
+-rw-r--r--   0     1001      123    10592 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/pager.rs
+-rw-r--r--   0     1001      123     2820 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/uri.rs
+-rw-r--r--   0     1001      123     6340 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gcs/writer.rs
+-rw-r--r--   0     1001      123     3648 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/backend.rs
+-rw-r--r--   0     1001      123     4276 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/builder.rs
+-rw-r--r--   0     1001      123     7046 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/core.rs
+-rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/error.rs
+-rw-r--r--   0     1001      123      904 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/mod.rs
+-rw-r--r--   0     1001      123     1981 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/writer.rs
+-rw-r--r--   0     1001      123    20887 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/backend.rs
+-rw-r--r--   0     1001      123     1908 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/error.rs
+-rw-r--r--   0     1001      123      877 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/mod.rs
+-rw-r--r--   0     1001      123     2375 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ghac/writer.rs
+-rw-r--r--   0     1001      123    16113 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/backend.rs
+-rw-r--r--   0     1001      123     1497 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/error.rs
+-rw-r--r--   0     1001      123      888 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/mod.rs
+-rw-r--r--   0     1001      123     3315 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/pager.rs
+-rw-r--r--   0     1001      123     2461 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/writer.rs
+-rw-r--r--   0     1001      123    16387 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/backend.rs
+-rw-r--r--   0     1001      123     1875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/error.rs
+-rw-r--r--   0     1001      123      265 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/fixtures/nginx.conf
+-rw-r--r--   0     1001      123      865 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/http/mod.rs
+-rw-r--r--   0     1001      123    17104 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/backend.rs
+-rw-r--r--   0     1001      123     1871 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/error.rs
+-rw-r--r--   0     1001      123     8200 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/ipld.rs
+-rw-r--r--   0     1001      123      875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/mod.rs
+-rw-r--r--   0     1001      123     9272 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/backend.rs
+-rw-r--r--   0     1001      123     3946 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/builder.rs
+-rw-r--r--   0     1001      123     2790 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/error.rs
+-rw-r--r--   0     1001      123      903 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/mod.rs
+-rw-r--r--   0     1001      123     3819 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/pager.rs
+-rw-r--r--   0     1001      123     1753 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/writer.rs
+-rw-r--r--   0     1001      123     5712 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memcached/ascii.rs
+-rw-r--r--   0     1001      123     9250 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memcached/backend.rs
+-rw-r--r--   0     1001      123      875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memcached/mod.rs
+-rw-r--r--   0     1001      123     4434 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memory/backend.rs
+-rw-r--r--   0     1001      123      857 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/memory/mod.rs
+-rw-r--r--   0     1001      123     4157 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/mod.rs
+-rw-r--r--   0     1001      123     8174 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/moka/backend.rs
+-rw-r--r--   0     1001      123      853 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/moka/mod.rs
+-rw-r--r--   0     1001      123    15197 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/backend.rs
+-rw-r--r--   0     1001      123     8411 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/core.rs
+-rw-r--r--   0     1001      123     3492 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/error.rs
+-rw-r--r--   0     1001      123      896 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/mod.rs
+-rw-r--r--   0     1001      123     6027 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/pager.rs
+-rw-r--r--   0     1001      123     2057 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/obs/writer.rs
+-rw-r--r--   0     1001      123    14620 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/backend.rs
+-rw-r--r--   0     1001      123     4177 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/error.rs
+-rw-r--r--   0     1001      123     9228 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/graph_model.rs
+-rw-r--r--   0     1001      123      926 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/mod.rs
+-rw-r--r--   0     1001      123     4874 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/pager.rs
+-rw-r--r--   0     1001      123     6253 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/writer.rs
+-rw-r--r--   0     1001      123     4895 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/appender.rs
+-rw-r--r--   0     1001      123    23406 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/backend.rs
+-rw-r--r--   0     1001      123    25647 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/core.rs
+-rw-r--r--   0     1001      123     3407 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/error.rs
+-rw-r--r--   0     1001      123      910 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/mod.rs
+-rw-r--r--   0     1001      123     7006 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/pager.rs
+-rw-r--r--   0     1001      123     6676 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/oss/writer.rs
+-rw-r--r--   0     1001      123    10722 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/redis/backend.rs
+-rw-r--r--   0     1001      123      855 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/redis/mod.rs
+-rw-r--r--   0     1001      123     5749 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/backend.rs
+-rw-r--r--   0     1001      123      859 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/mod.rs
+-rw-r--r--   0     1001      123    42100 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/backend.rs
+-rw-r--r--   0     1001      123     3395 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/compatible_services.md
+-rw-r--r--   0     1001      123    28632 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/core.rs
+-rw-r--r--   0     1001      123     4749 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/error.rs
+-rw-r--r--   0     1001      123      894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/mod.rs
+-rw-r--r--   0     1001      123     7387 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/pager.rs
+-rw-r--r--   0     1001      123     7259 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/s3/writer.rs
+-rw-r--r--   0     1001      123    16772 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/backend.rs
+-rw-r--r--   0     1001      123     2587 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/error.rs
+-rw-r--r--   0     1001      123      899 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/mod.rs
+-rw-r--r--   0     1001      123     2420 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/pager.rs
+-rw-r--r--   0     1001      123     3641 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/utils.rs
+-rw-r--r--   0     1001      123     1519 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sftp/writer.rs
+-rw-r--r--   0     1001      123     5603 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sled/backend.rs
+-rw-r--r--   0     1001      123      854 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/sled/mod.rs
+-rw-r--r--   0     1001      123     9798 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/backend.rs
+-rw-r--r--   0     1001      123     8021 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/core.rs
+-rw-r--r--   0     1001      123     2582 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/error.rs
+-rw-r--r--   0     1001      123      894 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/mod.rs
+-rw-r--r--   0     1001      123     2382 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/supabase/writer.rs
+-rw-r--r--   0     1001      123     4936 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs
+-rw-r--r--   0     1001      123     3636 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs
+-rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs
+-rw-r--r--   0     1001      123      912 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs
+-rw-r--r--   0     1001      123     2055 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs
+-rw-r--r--   0     1001      123    39360 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/backend.rs
+-rw-r--r--   0     1001      123    29776 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/core.rs
+-rw-r--r--   0     1001      123     3761 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/error.rs
+-rw-r--r--   0     1001      123      902 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/mod.rs
+-rw-r--r--   0     1001      123     7061 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/pager.rs
+-rw-r--r--   0     1001      123     2050 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/writer.rs
+-rw-r--r--   0     1001      123    20987 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/backend.rs
+-rw-r--r--   0     1001      123     1743 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/error.rs
+-rw-r--r--   0     1001      123      130 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/htpasswd
+-rw-r--r--   0     1001      123      626 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf
+-rw-r--r--   0     1001      123      531 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf
+-rw-r--r--   0     1001      123    16965 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/list_response.rs
+-rw-r--r--   0     1001      123      911 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/mod.rs
+-rw-r--r--   0     1001      123     2560 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/pager.rs
+-rw-r--r--   0     1001      123     2066 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webdav/writer.rs
+-rw-r--r--   0     1001      123    19875 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/backend.rs
+-rw-r--r--   0     1001      123     4085 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/error.rs
+-rw-r--r--   0     1001      123     4679 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/message.rs
+-rw-r--r--   0     1001      123      907 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/mod.rs
+-rw-r--r--   0     1001      123     2452 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/pager.rs
+-rw-r--r--   0     1001      123     2076 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/writer.rs
+-rw-r--r--   0     1001      123     8622 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/appender.rs
+-rw-r--r--   0     1001      123     2649 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/builder.rs
+-rw-r--r--   0     1001      123     6870 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/capability.rs
+-rw-r--r--   0     1001      123     2494 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/entry.rs
+-rw-r--r--   0     1001      123    12002 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/error.rs
+-rw-r--r--   0     1001      123     7417 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/list.rs
+-rw-r--r--   0     1001      123    16557 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/metadata.rs
+-rw-r--r--   0     1001      123     1554 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/mod.rs
+-rw-r--r--   0     1001      123     1747 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/mode.rs
+-rw-r--r--   0     1001      123    24284 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs
+-rw-r--r--   0     1001      123    13497 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/builder.rs
+-rw-r--r--   0     1001      123     3073 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/metadata.rs
+-rw-r--r--   0     1001      123     1098 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/mod.rs
+-rw-r--r--   0     1001      123    48177 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/operator/operator.rs
+-rw-r--r--   0     1001      123    12114 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/ops.rs
+-rw-r--r--   0     1001      123     9571 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/reader.rs
+-rw-r--r--   0     1001      123     6741 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/scheme.rs
+-rw-r--r--   0     1001      123    10795 2023-05-23 08:09:35.000000 opendal-0.35.0/local_dependencies/opendal/src/types/writer.rs
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 opendal-0.35.0/Cargo.toml
+-rw-r--r--   0     1001      123      709 2023-05-23 08:09:35.000000 opendal-0.35.0/.gitignore
+-rw-r--r--   0     1001      123     2212 2023-05-23 08:09:35.000000 opendal-0.35.0/CONTRIBUTING.md
+-rw-r--r--   0     1001      123      982 2023-05-23 08:09:35.000000 opendal-0.35.0/README.md
+-rw-r--r--   0     1001      123      765 2023-05-23 08:09:35.000000 opendal-0.35.0/benchmark/README.md
+-rw-r--r--   0     1001      123     2426 2023-05-23 08:09:35.000000 opendal-0.35.0/benchmark/async_opendal_benchmark.py
+-rw-r--r--   0     1001      123     2955 2023-05-23 08:09:35.000000 opendal-0.35.0/benchmark/async_origin_s3_benchmark_with_gevent.py
+-rw-r--r--   0     1001      123      917 2023-05-23 08:09:35.000000 opendal-0.35.0/examples/object.ipynb
+-rw-r--r--   0     1001      123     1665 2023-05-23 08:09:35.000000 opendal-0.35.0/pyproject.toml
+-rw-r--r--   0     1001      123      866 2023-05-23 08:09:35.000000 opendal-0.35.0/python/opendal/__init__.py
+-rw-r--r--   0     1001      123     2917 2023-05-23 08:09:35.000000 opendal-0.35.0/python/opendal/__init__.pyi
+-rw-r--r--   0     1001      123      405 2023-05-23 08:09:35.000000 opendal-0.35.0/python/opendal/layers.pyi
+-rw-r--r--   0     1001      123    11963 2023-05-23 08:09:35.000000 opendal-0.35.0/src/asyncio.rs
+-rw-r--r--   0     1001      123     3074 2023-05-23 08:09:35.000000 opendal-0.35.0/src/layers.rs
+-rw-r--r--   0     1001      123    12218 2023-05-23 08:09:35.000000 opendal-0.35.0/src/lib.rs
+-rw-r--r--   0     1001      123     1604 2023-05-23 08:09:35.000000 opendal-0.35.0/tests/binding.feature
+-rw-r--r--   0     1001      123     2942 2023-05-23 08:09:35.000000 opendal-0.35.0/tests/steps/binding.py
+-rw-r--r--   0     1001      123   131969 2023-05-23 08:09:35.000000 opendal-0.35.0/Cargo.lock
+-rw-r--r--   0        0        0     2151 1970-01-01 00:00:00.000000 opendal-0.35.0/PKG-INFO
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/Cargo.toml` & `opendal-0.35.0/local_dependencies/opendal/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,24 +24,25 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.34.0"
+version= "0.35.0"
 
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 default = [
   "rustls",
   "services-azblob",
   "services-azdfs",
+  "services-cos",
   "services-fs",
   "services-gcs",
   "services-ghac",
   "services-http",
   "services-ipmfs",
   "services-memory",
   "services-obs",
@@ -96,14 +97,19 @@
   "reqsign?/reqwest_request",
 ]
 services-azdfs = [
   "dep:reqsign",
   "reqsign?/services-azblob",
   "reqsign?/reqwest_request",
 ]
+services-cos = [
+  "dep:reqsign",
+  "reqsign?/services-tencent",
+  "reqsign?/reqwest_request",
+]
 services-dashmap = ["dep:dashmap"]
 services-fs = ["tokio/fs"]
 services-ftp = ["dep:suppaftp", "dep:lazy-regex", "dep:bb8", "dep:async-tls"]
 services-gcs = [
   "dep:reqsign",
   "reqsign?/services-google",
   "reqsign?/reqwest_request",
@@ -131,20 +137,15 @@
 services-redis = ["dep:redis"]
 services-rocksdb = ["dep:rocksdb"]
 services-s3 = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
 ]
-services-sftp = [
-  "dep:openssh",
-  "dep:openssh-sftp-client",
-  "dep:bb8",
-  "dep:owning_ref",
-]
+services-sftp = ["dep:openssh", "dep:openssh-sftp-client", "dep:dirs"]
 services-sled = ["dep:sled"]
 services-supabase = []
 services-vercel-artifacts = []
 services-wasabi = [
   "dep:reqsign",
   "reqsign?/services-aws",
   "reqsign?/reqwest_request",
@@ -166,67 +167,53 @@
 async-trait = "0.1.68"
 backon = "0.4.0"
 base64 = "0.21"
 bb8 = { version = "0.8", optional = true }
 bytes = "1.2"
 chrono = "0.4.24"
 dashmap = { version = "5.4", optional = true }
+dirs = { version = "5.0.1", optional = true }
 flagset = "0.4"
-futures = { version = "0.3", features = ["alloc"] }
+futures = { version = "0.3", default-features = false, features = ["alloc"] }
 hdrs = { version = "0.2", optional = true, features = ["async_file"] }
 http = "0.2.5"
 hyper = "0.14"
 lazy-regex = { version = "2.5.0", optional = true }
 log = "0.4"
 madsim = { version = "0.2.21", optional = true }
 md-5 = "0.10"
 metrics = { version = "0.20", optional = true }
 minitrace = { version = "0.4.0", optional = true }
 moka = { version = "0.10", optional = true, features = ["future"] }
 once_cell = "1"
 openssh = { version = "0.9.9", optional = true }
-openssh-sftp-client = { version = "0.12.2", optional = true }
+openssh-sftp-client = { version = "0.13.5", optional = true, features = [
+  "openssh",
+  "tracing",
+] }
 opentelemetry = { version = "0.19.0", optional = true }
-owning_ref = { version = "0.4.1", optional = true }
 parking_lot = "0.12"
 percent-encoding = "2"
 pin-project = "1"
 prometheus = { version = "0.13", features = ["process"], optional = true }
 prost = { version = "0.11", optional = true }
 quick-xml = { version = "0.27", features = ["serialize", "overlapped-lists"] }
 rand = { version = "0.8", optional = true }
 redis = { version = "0.22", features = [
   "tokio-comp",
   "connection-manager",
 ], optional = true }
-reqsign = { version = "0.10.1", default-features = false, optional = true }
+reqsign = { version = "0.12.0", default-features = false, optional = true }
 reqwest = { version = "0.11.13", features = [
   "stream",
 ], default-features = false }
 rocksdb = { version = "0.20.1", default-features = false, optional = true }
 serde = { version = "1", features = ["derive"] }
 serde_json = "1"
 sled = { version = "0.34.7", optional = true }
 suppaftp = { version = "4.5", default-features = false, features = [
   "async-secure",
   "async-rustls",
 ], optional = true }
 tokio = "1.27"
 tracing = { version = "0.1", optional = true }
 uuid = { version = "1", features = ["serde", "v4"] }
-
-[dev-dependencies]
-criterion = { version = "0.4", features = ["async", "async_tokio"] }
-dotenvy = "0.15"
-opentelemetry = { version = "0.19", default-features = false, features = [
-  "trace",
-] }
-opentelemetry-jaeger = "0.18"
-paste = "1"
-pretty_assertions = "1"
-rand = "0.8"
-sha2 = "0.10"
-size = "0.4"
-tokio = { version = "1.27", features = ["fs", "macros", "rt-multi-thread"] }
-tracing-opentelemetry = "0.17"
-tracing-subscriber = { version = "0.3", features = ["env-filter"] }
-wiremock = "0.5"
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/CHANGELOG.md` & `opendal-0.35.0/local_dependencies/opendal/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,77 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](https://semver.org/).
 
+## [v0.35.0] - 2023-05-23
+
+### Added
+
+- feat(services/onedrive): Implement `list`, `create_dir`, `stat` and upload
+ing large files (#2231)
+- feat(bindings/C): Initially support stat in C binding (#2249)
+- feat(bindings/python): Enable `abi3` to avoid building on different python
+ version (#2255)
+- feat(bindings/C): support BDD tests using GTest (#2254)
+- feat(services/sftp): setup integration tests (#2192)
+- feat(core): Add trait and public API for `append` (#2260)
+- feat(services/sftp): support copy and rename for sftp (#2263)
+- feat(services/sftp): support copy and read_seek (#2267)
+- feat: Add COS service support (#2269)
+- feat(services/cos): Add support for loading from env (#2271)
+- feat(core): add presign support for obs (#2253)
+- feat(services/sftp): setup integration tests (#2192)
+- feat(core): add presign support for obs (#2253)
+- feat(core): public API of append (#2284)
+- test(core): test for append (#2286)
+- feat(services/oss): add append support (#2279)
+- feat(bindings/java): implement async ops to pass AsyncStepsTest (#2291)
+
+### Changed
+
+- services/gdrive: port code to GdriveCore & add path_2_id cache (#2203)
+- refactor: Minimize futures dependencies (#2248)
+- refactor: Add Operator::via_map to support init without generic type parameters (#2280)
+- refactor(binding/java): build, async and docs (#2276)
+
+### Fixed
+
+- fix: Fix bugs that failed wasabi's integration tests (#2273)
+
+### Removed
+
+- feat(core): remove `scan` from raw API (#2262)
+
+### Docs
+
+- chore(s3): update builder region doc (#2247)
+- docs: Add services in readme (#2251)
+- docs: Unify capabilities list for kv services (#2257)
+- docs(nodejs): fix some example code errors (#2277)
+- docs(bindings/C): C binding contributing documentation (#2266)
+- docs: Add new docs that available for all languages (#2285)
+- docs: Remove unlicensed svg (#2289)
+- fix(website): double active route (#2290)
+
+### CI
+
+- ci: Enable test for cos (#2270)
+- ci: Add integration tests for supabase (#2272)
+- ci: replace set-output for docs (#2275)
+- ci: Fix unit tests (#2282)
+- ci: Cleanup NOTICE file (#2281)
+- ci: Fix release not contains incubating (#2292)
+
+### Chore
+
+- chore(core): remove unnecessary path prefix (#2265)
+
 ## [v0.34.0] - 2023-05-09
 
 ### Added
 
 - feat(writer): configurable buffer size of unsized write (#2143)
 - feat(oay): Add basic s3 list_objects_v2 with start_after support (#2219)
 - feat: Add typed kv adapter and migrate moka to it (#2222)
@@ -2093,14 +2156,15 @@
 
 ## v0.0.1 - 2022-02-14
 
 ### Added
 
 Hello, OpenDAL!
 
+[v0.35.0]: https://github.com/apache/incubator-opendal/compare/v0.34.0...v0.35.0
 [v0.34.0]: https://github.com/apache/incubator-opendal/compare/v0.33.3...v0.34.0
 [v0.33.3]: https://github.com/apache/incubator-opendal/compare/v0.33.2...v0.33.3
 [v0.33.2]: https://github.com/apache/incubator-opendal/compare/v0.33.1...v0.33.2
 [v0.33.1]: https://github.com/apache/incubator-opendal/compare/v0.33.0...v0.33.1
 [v0.33.0]: https://github.com/apache/incubator-opendal/compare/v0.32.0...v0.33.0
 [v0.32.0]: https://github.com/apache/incubator-opendal/compare/v0.31.1...v0.32.0
 [v0.31.1]: https://github.com/apache/incubator-opendal/compare/v0.31.0...v0.31.1
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/CONTRIBUTING.md` & `opendal-0.35.0/local_dependencies/opendal/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/README.md` & `opendal-0.35.0/local_dependencies/opendal/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/benches/ops/README.md` & `opendal-0.35.0/local_dependencies/opendal/benches/ops/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/benches/ops/main.rs` & `opendal-0.35.0/local_dependencies/opendal/benches/ops/main.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/benches/ops/read.rs` & `opendal-0.35.0/local_dependencies/opendal/benches/ops/read.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/benches/ops/utils.rs` & `opendal-0.35.0/local_dependencies/opendal/benches/ops/utils.rs`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,25 @@
 
 fn service<AB: Builder>() -> Option<Operator> {
     let test_key = format!("opendal_{}_test", AB::SCHEME).to_uppercase();
     if env::var(test_key).unwrap_or_default() != "on" {
         return None;
     }
 
+    let prefix = format!("opendal_{}_", AB::SCHEME);
+    let envs = env::vars()
+        .filter_map(move |(k, v)| {
+            k.to_lowercase()
+                .strip_prefix(&prefix)
+                .map(|k| (k.to_string(), v))
+        })
+        .collect();
+
     Some(
-        Operator::from_env::<AB>()
+        Operator::from_map::<AB>(envs)
             .unwrap_or_else(|_| panic!("init {} must succeed", AB::SCHEME))
             .finish(),
     )
 }
 
 pub fn services() -> Vec<(&'static str, Option<Operator>)> {
     let _ = dotenvy::dotenv();
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/benches/ops/write.rs` & `opendal-0.35.0/local_dependencies/opendal/benches/ops/write.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/examples/object.rs` & `opendal-0.35.0/local_dependencies/opendal/examples/object.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/comparisons/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/comparisons/vs_object_store.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/concepts.rs` & `opendal-0.35.0/local_dependencies/opendal/src/docs/concepts.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/features.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/features.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/internals/accessor.rs` & `opendal-0.35.0/local_dependencies/opendal/src/docs/internals/accessor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/internals/layer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/docs/internals/layer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/internals/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/docs/internals/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/docs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0000_example.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0041_object_native_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0044_error_handle.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0057_auto_region.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0069_object_stream.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0090_limited_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0112_path_normalization.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0191_async_streaming_io.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0203_remove_credential.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0221_create_dir.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0247_retryable_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0293_object_id.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0337_dir_entry.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0409_accessor_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0413_presign.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0423_command_line_interface.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0429_init_from_iter.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0438_multipart.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0443_gateway.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0501_new_builder.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0554_write_refactor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0561_list_metadata_reuse.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0599_blocking_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0623_redis_service.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0627_split_capabilities.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0661_path_in_accessor.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0793_generic_kv_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0926_object_reader.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/0977_refactor_error.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1085_object_handler.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1391_object_metadataer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1398_query_based_metadata.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1420_object_writer.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1477_remove_object_concept.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/1735_operation_extension.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2083_writer_sink_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/2133_append_api.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/rfcs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/docs/rfcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/docs/upgrade.md` & `opendal-0.35.0/local_dependencies/opendal/src/docs/upgrade.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+# Upgrade to v0.35
+
+## Public API
+
+- OpenDAL removes rarely used `Operator::from_env` and `Operator::from_iter` APIs
+  - Users can use `Operator::via_map` instead.
+
+## Raw API
+
+- OpenDAL adds `append` support with could break existing layers. Please make sure `append` requests have been forward correctly.
+- After the merging of `scan` and `list`, OpenDAL removes the `scan` from raw API. Please use `list_without_delimiter` instead.
+
 # Upgrade to v0.34
 
 ## Public API
 
 - OpenDAL raises it's MSRV to 1.65 for dependences changes
 - `OperatorInfo::can_scan` has been removed, to check if underlying services support scan a dir natively, please use `Capability::list_without_delimiter` instead.
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/chaos.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/chaos.rs`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for ChaosAccessor<A> {
     type Inner = A;
     type Reader = ChaosReader<A::Reader>;
     type BlockingReader = ChaosReader<A::BlockingReader>;
     type Writer = A::Writer;
     type BlockingWriter = A::BlockingWriter;
+    type Appender = A::Appender;
     type Pager = A::Pager;
     type BlockingPager = A::BlockingPager;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -131,14 +132,18 @@
         self.inner.write(path, args).await
     }
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         self.inner.blocking_write(path, args)
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner.append(path, args).await
+    }
+
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         self.inner.list(path, args).await
     }
 
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
         self.inner.blocking_list(path, args)
     }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/complete.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/complete.rs`

 * *Files 21% similar despite different names*

```diff
@@ -323,14 +323,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for CompleteReaderAccessor<A> {
     type Inner = A;
     type Reader = CompleteReader<A, A::Reader>;
     type BlockingReader = CompleteReader<A, A::BlockingReader>;
     type Writer = CompleteWriter<A::Writer>;
     type BlockingWriter = CompleteWriter<A::BlockingWriter>;
+    type Appender = CompleteAppender<A::Appender>;
     type Pager = CompletePager<A, A::Pager>;
     type BlockingPager = CompletePager<A, A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -371,14 +372,21 @@
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         let size = args.content_length();
         self.inner
             .blocking_write(path, args)
             .map(|(rp, w)| (rp, CompleteWriter::new(w, size)))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner
+            .append(path, args)
+            .await
+            .map(|(rp, a)| (rp, CompleteAppender::new(a)))
+    }
+
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         self.complete_list(path, args).await
     }
 
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
         self.complete_blocking_list(path, args)
     }
@@ -642,7 +650,55 @@
         })?;
 
         w.close()?;
         self.inner = None;
         Ok(())
     }
 }
+
+pub struct CompleteAppender<A> {
+    inner: Option<A>,
+}
+
+impl<A> CompleteAppender<A> {
+    pub fn new(inner: A) -> CompleteAppender<A> {
+        CompleteAppender { inner: Some(inner) }
+    }
+}
+
+/// Check if the appender has been closed while debug_assertions enabled.
+/// This code will never be executed in release mode.
+#[cfg(debug_assertions)]
+impl<A> Drop for CompleteAppender<A> {
+    fn drop(&mut self) {
+        if self.inner.is_none() {
+            // Do we need to panic here?
+            log::warn!("appender has not been closed, must be a bug")
+        }
+    }
+}
+
+#[async_trait]
+impl<A> oio::Append for CompleteAppender<A>
+where
+    A: oio::Append,
+{
+    async fn append(&mut self, bs: Bytes) -> Result<()> {
+        let a = self
+            .inner
+            .as_mut()
+            .ok_or_else(|| Error::new(ErrorKind::Unexpected, "appender has been closed"))?;
+
+        a.append(bs).await
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        let a = self
+            .inner
+            .as_mut()
+            .ok_or_else(|| Error::new(ErrorKind::Unexpected, "appender has been closed"))?;
+
+        a.close().await?;
+        self.inner = None;
+        Ok(())
+    }
+}
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/concurrent_limit.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/concurrent_limit.rs`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for ConcurrentLimitAccessor<A> {
     type Inner = A;
     type Reader = ConcurrentLimitWrapper<A::Reader>;
     type BlockingReader = ConcurrentLimitWrapper<A::BlockingReader>;
     type Writer = ConcurrentLimitWrapper<A::Writer>;
     type BlockingWriter = ConcurrentLimitWrapper<A::BlockingWriter>;
+    type Appender = ConcurrentLimitWrapper<A::Appender>;
     type Pager = ConcurrentLimitWrapper<A::Pager>;
     type BlockingPager = ConcurrentLimitWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -128,14 +129,28 @@
 
         self.inner
             .write(path, args)
             .await
             .map(|(rp, w)| (rp, ConcurrentLimitWrapper::new(w, permit)))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        let permit = self
+            .semaphore
+            .clone()
+            .acquire_owned()
+            .await
+            .expect("semaphore must be valid");
+
+        self.inner
+            .append(path, args)
+            .await
+            .map(|(rp, a)| (rp, ConcurrentLimitWrapper::new(a, permit)))
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         let _permit = self
             .semaphore
             .acquire()
             .await
             .expect("semaphore must be valid");
 
@@ -306,14 +321,25 @@
 
     fn close(&mut self) -> Result<()> {
         self.inner.close()
     }
 }
 
 #[async_trait]
+impl<R: oio::Append> oio::Append for ConcurrentLimitWrapper<R> {
+    async fn append(&mut self, bs: Bytes) -> Result<()> {
+        self.inner.append(bs).await
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        self.inner.close().await
+    }
+}
+
+#[async_trait]
 impl<R: oio::Page> oio::Page for ConcurrentLimitWrapper<R> {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         self.inner.next().await
     }
 }
 
 impl<R: oio::BlockingPage> oio::BlockingPage for ConcurrentLimitWrapper<R> {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/error_context.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/error_context.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 use std::task::Poll;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use futures::TryFutureExt;
 
 use crate::ops::*;
+use crate::raw::oio::AppendOperation;
 use crate::raw::oio::PageOperation;
 use crate::raw::oio::ReadOperation;
 use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
 
 /// ErrorContextLayer will add error context into all layers.
@@ -67,14 +68,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for ErrorContextAccessor<A> {
     type Inner = A;
     type Reader = ErrorContextWrapper<A::Reader>;
     type BlockingReader = ErrorContextWrapper<A::BlockingReader>;
     type Writer = ErrorContextWrapper<A::Writer>;
     type BlockingWriter = ErrorContextWrapper<A::BlockingWriter>;
+    type Appender = ErrorContextWrapper<A::Appender>;
     type Pager = ErrorContextWrapper<A::Pager>;
     type BlockingPager = ErrorContextWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -134,14 +136,35 @@
                 err.with_operation(Operation::Write)
                     .with_context("service", self.meta.scheme())
                     .with_context("path", path)
             })
             .await
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner
+            .append(path, args)
+            .map_ok(|(rp, os)| {
+                (
+                    rp,
+                    ErrorContextWrapper {
+                        scheme: self.meta.scheme(),
+                        path: path.to_string(),
+                        inner: os,
+                    },
+                )
+            })
+            .map_err(|err| {
+                err.with_operation(Operation::Append)
+                    .with_context("service", self.meta.scheme())
+                    .with_context("path", path)
+            })
+            .await
+    }
+
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         self.inner
             .copy(from, to, args)
             .map_err(|err| {
                 err.with_operation(Operation::Copy)
                     .with_context("service", self.meta.scheme())
                     .with_context("from", from)
@@ -444,14 +467,33 @@
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
     }
 }
 
 #[async_trait::async_trait]
+impl<T: oio::Append> oio::Append for ErrorContextWrapper<T> {
+    async fn append(&mut self, bs: Bytes) -> Result<()> {
+        self.inner.append(bs).await.map_err(|err| {
+            err.with_operation(AppendOperation::Append)
+                .with_context("service", self.scheme)
+                .with_context("path", &self.path)
+        })
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        self.inner.close().await.map_err(|err| {
+            err.with_operation(AppendOperation::Close)
+                .with_context("service", self.scheme)
+                .with_context("path", &self.path)
+        })
+    }
+}
+
+#[async_trait::async_trait]
 impl<T: oio::Page> oio::Page for ErrorContextWrapper<T> {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         self.inner.next().await.map_err(|err| {
             err.with_operation(PageOperation::Next)
                 .with_context("service", self.scheme)
                 .with_context("path", &self.path)
         })
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/immutable_index.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/immutable_index.rs`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 /// Add an immutable in-memory index for underlying storage services.
 ///
 /// Especially useful for services without list capability like HTTP.
 ///
 /// # Examples
 ///
 /// ```rust, no_run
+/// use std::collections::HashMap;
+///
 /// use opendal::layers::ImmutableIndexLayer;
 /// use opendal::services;
 /// use opendal::Operator;
 ///
 /// let mut iil = ImmutableIndexLayer::default();
 ///
 /// for i in ["file", "dir/", "dir/file", "dir_without_prefix/file"] {
 ///     iil.insert(i.to_string())
 /// }
 ///
-/// let op = Operator::from_env::<services::Http>()
+/// let op = Operator::from_map::<services::Http>(HashMap::default())
 ///     .unwrap()
 ///     .layer(iil)
 ///     .finish();
 /// ```
 #[derive(Default, Debug, Clone)]
 pub struct ImmutableIndexLayer {
     vec: Vec<String>,
@@ -135,14 +137,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for ImmutableIndexAccessor<A> {
     type Inner = A;
     type Reader = A::Reader;
     type BlockingReader = A::BlockingReader;
     type Writer = A::Writer;
     type BlockingWriter = A::BlockingWriter;
+    type Appender = A::Appender;
     type Pager = ImmutableDir;
     type BlockingPager = ImmutableDir;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -190,14 +193,18 @@
         self.inner.write(path, args).await
     }
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         self.inner.blocking_write(path, args)
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner.append(path, args).await
+    }
+
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
         let mut path = path;
         if path == "/" {
             path = ""
         }
 
         let idx = if args.delimiter() == "/" {
@@ -280,17 +287,20 @@
         let _ = tracing_subscriber::fmt().with_test_writer().try_init();
 
         let mut iil = ImmutableIndexLayer::default();
         for i in ["file", "dir/", "dir/file", "dir_without_prefix/file"] {
             iil.insert(i.to_string())
         }
 
-        let op = Operator::new(Http::from_iter(
-            vec![("endpoint".to_string(), "https://xuanwo.io".to_string())].into_iter(),
-        ))?
+        let op = Operator::new(Http::from_map({
+            let mut map = HashMap::new();
+            map.insert("endpoint".to_string(), "https://xuanwo.io".to_string());
+
+            map
+        }))?
         .layer(LoggingLayer::default())
         .layer(iil)
         .finish();
 
         let mut map = HashMap::new();
         let mut set = HashSet::new();
         let mut ds = op.list("").await?;
@@ -318,17 +328,20 @@
         let _ = tracing_subscriber::fmt().with_test_writer().try_init();
 
         let mut iil = ImmutableIndexLayer::default();
         for i in ["file", "dir/", "dir/file", "dir_without_prefix/file"] {
             iil.insert(i.to_string())
         }
 
-        let op = Operator::new(Http::from_iter(
-            vec![("endpoint".to_string(), "https://xuanwo.io".to_string())].into_iter(),
-        ))?
+        let op = Operator::new(Http::from_map({
+            let mut map = HashMap::new();
+            map.insert("endpoint".to_string(), "https://xuanwo.io".to_string());
+
+            map
+        }))?
         .layer(LoggingLayer::default())
         .layer(iil)
         .finish();
 
         let mut ds = op.scan("/").await?;
         let mut set = HashSet::new();
         let mut map = HashMap::new();
@@ -362,17 +375,20 @@
             "dataset/stateful/ontime_2007_200.csv",
             "dataset/stateful/ontime_2008_200.csv",
             "dataset/stateful/ontime_2009_200.csv",
         ] {
             iil.insert(i.to_string())
         }
 
-        let op = Operator::new(Http::from_iter(
-            vec![("endpoint".to_string(), "https://xuanwo.io".to_string())].into_iter(),
-        ))?
+        let op = Operator::new(Http::from_map({
+            let mut map = HashMap::new();
+            map.insert("endpoint".to_string(), "https://xuanwo.io".to_string());
+
+            map
+        }))?
         .layer(LoggingLayer::default())
         .layer(iil)
         .finish();
 
         //  List /
         let mut map = HashMap::new();
         let mut set = HashSet::new();
@@ -423,17 +439,20 @@
             "dataset/stateful/ontime_2007_200.csv",
             "dataset/stateful/ontime_2008_200.csv",
             "dataset/stateful/ontime_2009_200.csv",
         ] {
             iil.insert(i.to_string())
         }
 
-        let op = Operator::new(Http::from_iter(
-            vec![("endpoint".to_string(), "https://xuanwo.io".to_string())].into_iter(),
-        ))?
+        let op = Operator::new(Http::from_map({
+            let mut map = HashMap::new();
+            map.insert("endpoint".to_string(), "https://xuanwo.io".to_string());
+
+            map
+        }))?
         .layer(LoggingLayer::default())
         .layer(iil)
         .finish();
 
         let mut ds = op.scan("/").await?;
 
         let mut map = HashMap::new();
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/logging.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/logging.rs`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for LoggingAccessor<A> {
     type Inner = A;
     type Reader = LoggingReader<A::Reader>;
     type BlockingReader = LoggingReader<A::BlockingReader>;
     type Writer = LoggingWriter<A::Writer>;
     type BlockingWriter = LoggingWriter<A::BlockingWriter>;
+    type Appender = LoggingAppender<A::Appender>;
     type Pager = LoggingPager<A::Pager>;
     type BlockingPager = LoggingPager<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -336,14 +337,59 @@
                         self.err_status(&err)
                     )
                 };
                 err
             })
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        debug!(
+            target: LOGGING_TARGET,
+            "service={} operation={} path={} -> started",
+            self.scheme,
+            Operation::Append,
+            path
+        );
+
+        self.inner
+            .append(path, args)
+            .await
+            .map(|(rp, a)| {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} path={} -> start appending",
+                    self.scheme,
+                    Operation::Append,
+                    path,
+                );
+                let a = LoggingAppender::new(
+                    self.scheme,
+                    Operation::Append,
+                    path,
+                    a,
+                    self.failure_level,
+                );
+                (rp, a)
+            })
+            .map_err(|err| {
+                if let Some(lvl) = self.err_level(&err) {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} path={} -> {}: {err:?}",
+                        self.scheme,
+                        Operation::Append,
+                        path,
+                        self.err_status(&err)
+                    )
+                };
+                err
+            })
+    }
+
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         debug!(
             target: LOGGING_TARGET,
             "service={} operation={} from={} to={} -> started",
             self.scheme,
             Operation::Copy,
             from,
@@ -1419,14 +1465,106 @@
                     )
                 }
                 Err(err)
             }
         }
     }
 }
+
+pub struct LoggingAppender<A> {
+    scheme: Scheme,
+    op: Operation,
+    path: String,
+
+    failure_level: Option<Level>,
+
+    inner: A,
+}
+
+impl<A> LoggingAppender<A> {
+    fn new(
+        scheme: Scheme,
+        op: Operation,
+        path: &str,
+        appender: A,
+        failure_level: Option<Level>,
+    ) -> Self {
+        Self {
+            scheme,
+            op,
+            path: path.to_string(),
+
+            failure_level,
+
+            inner: appender,
+        }
+    }
+}
+
+#[async_trait]
+impl<A: oio::Append> oio::Append for LoggingAppender<A> {
+    async fn append(&mut self, bs: Bytes) -> Result<()> {
+        let len = bs.len();
+
+        match self.inner.append(bs).await {
+            Ok(_) => {
+                trace!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} path={} -> data append {}B",
+                    self.scheme,
+                    self.op,
+                    self.path,
+                    len
+                );
+                Ok(())
+            }
+            Err(err) => {
+                if let Some(lvl) = self.failure_level {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} path={} -> data append failed: {err:?}",
+                        self.scheme,
+                        self.op,
+                        self.path,
+                    )
+                }
+                Err(err)
+            }
+        }
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        match self.inner.close().await {
+            Ok(_) => {
+                debug!(
+                    target: LOGGING_TARGET,
+                    "service={} operation={} path={} -> data appended finished",
+                    self.scheme,
+                    self.op,
+                    self.path,
+                );
+                Ok(())
+            }
+            Err(err) => {
+                if let Some(lvl) = self.failure_level {
+                    log!(
+                        target: LOGGING_TARGET,
+                        lvl,
+                        "service={} operation={} path={} -> data appender close failed: {err:?}",
+                        self.scheme,
+                        self.op,
+                        self.path,
+                    )
+                }
+                Err(err)
+            }
+        }
+    }
+}
 
 pub struct LoggingPager<P> {
     scheme: Scheme,
     path: String,
     op: Operation,
 
     finished: bool,
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/madsim.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/madsim.rs`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
 #[async_trait]
 impl LayeredAccessor for MadsimAccessor {
     type Inner = ();
     type Reader = MadsimReader;
     type BlockingReader = ();
     type Writer = MadsimWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = MadsimPager;
     type BlockingPager = ();
 
     fn inner(&self) -> &Self::Inner {
         &()
     }
 
@@ -217,14 +218,25 @@
         }
         #[cfg(not(madsim))]
         {
             unreachable!("madsim is not enabled")
         }
     }
 
+    async fn append(
+        &self,
+        path: &str,
+        args: OpAppend,
+    ) -> crate::Result<(RpAppend, Self::Appender)> {
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "will not be supported in MadsimLayer",
+        ))
+    }
+
     async fn list(&self, path: &str, args: OpList) -> crate::Result<(RpList, Self::Pager)> {
         Err(Error::new(
             ErrorKind::Unsupported,
             "will be supported in the future",
         ))
     }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/metrics.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/metrics.rs`

 * *Files 0% similar despite different names*

```diff
@@ -409,14 +409,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for MetricsAccessor<A> {
     type Inner = A;
     type Reader = MetricWrapper<A::Reader>;
     type BlockingReader = MetricWrapper<A::BlockingReader>;
     type Writer = MetricWrapper<A::Writer>;
     type BlockingWriter = MetricWrapper<A::BlockingWriter>;
+    type Appender = A::Appender;
     type Pager = A::Pager;
     type BlockingPager = A::BlockingPager;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -506,14 +507,18 @@
             .inspect_err(|e| {
                 self.handle
                     .increment_errors_total(Operation::Write, e.kind());
             })
             .await
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner.append(path, args).await
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.handle.requests_total_stat.increment(1);
 
         let start = Instant::now();
 
         self.inner
             .stat(path, args)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/minitrace.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/minitrace.rs`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for MinitraceAccessor<A> {
     type Inner = A;
     type Reader = MinitraceWrapper<A::Reader>;
     type BlockingReader = MinitraceWrapper<A::BlockingReader>;
     type Writer = MinitraceWrapper<A::Writer>;
     type BlockingWriter = MinitraceWrapper<A::BlockingWriter>;
+    type Appender = A::Appender;
     type Pager = MinitraceWrapper<A::Pager>;
     type BlockingPager = MinitraceWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -164,14 +165,18 @@
         let span = Span::enter_with_local_parent("write");
         self.inner
             .write(path, args)
             .map(|v| v.map(|(rp, r)| (rp, MinitraceWrapper::new(span, r))))
             .await
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner.append(path, args).await
+    }
+
     #[trace("copy", enter_on_poll = true)]
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         self.inner().copy(from, to, args).await
     }
 
     #[trace("rename", enter_on_poll = true)]
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/oteltrace.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/oteltrace.rs`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for OtelTraceAccessor<A> {
     type Inner = A;
     type Reader = OtelTraceWrapper<A::Reader>;
     type BlockingReader = OtelTraceWrapper<A::BlockingReader>;
     type Writer = OtelTraceWrapper<A::Writer>;
     type BlockingWriter = OtelTraceWrapper<A::BlockingWriter>;
+    type Appender = A::Appender;
     type Pager = OtelTraceWrapper<A::Pager>;
     type BlockingPager = OtelTraceWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -112,14 +113,18 @@
         span.set_attribute(KeyValue::new("args", format!("{:?}", args)));
         self.inner
             .write(path, args)
             .await
             .map(|(rp, r)| (rp, OtelTraceWrapper::new(span, r)))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner.append(path, args).await
+    }
+
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         let tracer = global::tracer("opendal");
         let mut span = tracer.start("copy");
         span.set_attribute(KeyValue::new("from", from.to_string()));
         span.set_attribute(KeyValue::new("to", to.to_string()));
         span.set_attribute(KeyValue::new("args", format!("{:?}", args)));
         let cx = Context::current_with_span(span);
@@ -299,15 +304,15 @@
 }
 
 impl<R: oio::BlockingRead> oio::BlockingRead for OtelTraceWrapper<R> {
     fn read(&mut self, buf: &mut [u8]) -> Result<usize> {
         self.inner.read(buf)
     }
 
-    fn seek(&mut self, pos: std::io::SeekFrom) -> Result<u64> {
+    fn seek(&mut self, pos: io::SeekFrom) -> Result<u64> {
         self.inner.seek(pos)
     }
 
     fn next(&mut self) -> Option<Result<Bytes>> {
         self.inner.next()
     }
 }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/prometheus.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/prometheus.rs`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for PrometheusAccessor<A> {
     type Inner = A;
     type Reader = PrometheusMetricWrapper<A::Reader>;
     type BlockingReader = PrometheusMetricWrapper<A::BlockingReader>;
     type Writer = PrometheusMetricWrapper<A::Writer>;
     type BlockingWriter = PrometheusMetricWrapper<A::BlockingWriter>;
+    type Appender = A::Appender;
     type Pager = A::Pager;
     type BlockingPager = A::BlockingPager;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -294,14 +295,18 @@
         write_res.map_err(|e| {
             self.stats
                 .increment_errors_total(Operation::Write, e.kind());
             e
         })
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner.append(path, args).await
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         self.stats
             .requests_total
             .with_label_values(&[&self.scheme, Operation::Stat.into_static()])
             .inc();
         let timer = self
             .stats
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/retry.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/retry.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 use backon::ExponentialBuilder;
 use backon::Retryable;
 use bytes::Bytes;
 use futures::FutureExt;
 use log::warn;
 
 use crate::ops::*;
+use crate::raw::oio::AppendOperation;
 use crate::raw::oio::PageOperation;
 use crate::raw::oio::ReadOperation;
 use crate::raw::oio::WriteOperation;
 use crate::raw::*;
 use crate::*;
 
 /// Add retry for temporary failed operations.
@@ -157,14 +158,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for RetryAccessor<A> {
     type Inner = A;
     type Reader = RetryWrapper<A::Reader>;
     type BlockingReader = RetryWrapper<A::BlockingReader>;
     type Writer = RetryWrapper<A::Writer>;
     type BlockingWriter = RetryWrapper<A::BlockingWriter>;
+    type Appender = RetryWrapper<A::Appender>;
     type Pager = RetryWrapper<A::Pager>;
     type BlockingPager = RetryWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -215,14 +217,31 @@
             .map(|v| {
                 v.map(|(rp, r)| (rp, RetryWrapper::new(r, path, self.builder.clone())))
                     .map_err(|e| e.set_persistent())
             })
             .await
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        { || self.inner.append(path, args.clone()) }
+            .retry(&self.builder)
+            .when(|e| e.is_temporary())
+            .notify(|err, dur| {
+                warn!(
+                    target: "opendal::service",
+                    "operation={} -> retry after {}s: error={:?}",
+                    Operation::Append, dur.as_secs_f64(), err)
+            })
+            .map(|v| {
+                v.map(|(rp, r)| (rp, RetryWrapper::new(r, path, self.builder.clone())))
+                    .map_err(|e| e.set_persistent())
+            })
+            .await
+    }
+
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         { || self.inner.stat(path, args.clone()) }
             .retry(&self.builder)
             .when(|e| e.is_temporary())
             .notify(|err, dur| {
                 warn!(
                     target: "opendal::service",
@@ -700,14 +719,59 @@
             })
             .call()
             .map_err(|e| e.set_persistent())
     }
 }
 
 #[async_trait]
+impl<A: oio::Append> oio::Append for RetryWrapper<A> {
+    async fn append(&mut self, bs: Bytes) -> Result<()> {
+        let mut backoff = self.builder.build();
+
+        loop {
+            match self.inner.append(bs.clone()).await {
+                Ok(v) => return Ok(v),
+                Err(e) if !e.is_temporary() => return Err(e),
+                Err(e) => match backoff.next() {
+                    None => return Err(e),
+                    Some(dur) => {
+                        warn!(target: "opendal::service",
+                              "operation={} path={} -> appender retry after {}s: error={:?}",
+                              AppendOperation::Append, self.path, dur.as_secs_f64(), e);
+                        tokio::time::sleep(dur).await;
+                        continue;
+                    }
+                },
+            }
+        }
+    }
+
+    async fn close(&mut self) -> Result<()> {
+        let mut backoff = self.builder.build();
+
+        loop {
+            match self.inner.close().await {
+                Ok(v) => return Ok(v),
+                Err(e) if !e.is_temporary() => return Err(e),
+                Err(e) => match backoff.next() {
+                    None => return Err(e),
+                    Some(dur) => {
+                        warn!(target: "opendal::service",
+                              "operation={} path={} -> appender retry after {}s: error={:?}",
+                              AppendOperation::Close, self.path, dur.as_secs_f64(), e);
+                        tokio::time::sleep(dur).await;
+                        continue;
+                    }
+                },
+            }
+        }
+    }
+}
+
+#[async_trait]
 impl<P: oio::Page> oio::Page for RetryWrapper<P> {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
         let mut backoff = self.builder.build();
 
         loop {
             match self.inner.next().await {
                 Ok(v) => return Ok(v),
@@ -786,14 +850,15 @@
 
     #[async_trait]
     impl Accessor for MockService {
         type Reader = MockReader;
         type BlockingReader = ();
         type Writer = ();
         type BlockingWriter = ();
+        type Appender = ();
         type Pager = MockPager;
         type BlockingPager = ();
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
             am.set_capability(Capability {
                 list: true,
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/tracing.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/tracing.rs`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for TracingAccessor<A> {
     type Inner = A;
     type Reader = TracingWrapper<A::Reader>;
     type BlockingReader = TracingWrapper<A::BlockingReader>;
     type Writer = TracingWrapper<A::Writer>;
     type BlockingWriter = TracingWrapper<A::BlockingWriter>;
+    type Appender = A::Appender;
     type Pager = TracingWrapper<A::Pager>;
     type BlockingPager = TracingWrapper<A::BlockingPager>;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -167,14 +168,18 @@
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         self.inner
             .write(path, args)
             .await
             .map(|(rp, r)| (rp, TracingWrapper::new(Span::current(), r)))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner.append(path, args).await
+    }
+
     #[tracing::instrument(level = "debug", skip(self))]
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         self.inner().copy(from, to, args).await
     }
 
     #[tracing::instrument(level = "debug", skip(self))]
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/layers/type_eraser.rs` & `opendal-0.35.0/local_dependencies/opendal/src/layers/type_eraser.rs`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 #[async_trait]
 impl<A: Accessor> LayeredAccessor for TypeEraseAccessor<A> {
     type Inner = A;
     type Reader = oio::Reader;
     type BlockingReader = oio::BlockingReader;
     type Writer = oio::Writer;
     type BlockingWriter = oio::BlockingWriter;
+    type Appender = oio::Appender;
     type Pager = oio::Pager;
     type BlockingPager = oio::BlockingPager;
 
     fn inner(&self) -> &Self::Inner {
         &self.inner
     }
 
@@ -87,14 +88,21 @@
 
     fn blocking_write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::BlockingWriter)> {
         self.inner
             .blocking_write(path, args)
             .map(|(rp, w)| (rp, Box::new(w) as oio::BlockingWriter))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.inner
+            .append(path, args)
+            .await
+            .map(|(rp, a)| (rp, Box::new(a) as oio::Appender))
+    }
+
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         self.inner
             .list(path, args)
             .await
             .map(|(rp, p)| (rp, Box::new(p) as oio::Pager))
     }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/lib.rs` & `opendal-0.35.0/local_dependencies/opendal/src/lib.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/accessor.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/accessor.rs`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     /// `blocking_write` operation.
     type BlockingWriter: oio::BlockingWrite;
     /// Pager is the associated page that return in `list` operation.
     type Pager: oio::Page;
     /// BlockingPager is the associated pager that could return in
     /// `blocking_list` operation.
     type BlockingPager: oio::BlockingPage;
+    /// Appender is the associated appender that could return in `append` operation.
+    type Appender: oio::Append;
 
     /// Invoke the `info` operation to get metadata of accessor.
     ///
     /// # Notes
     ///
     /// This function is required to be implemented.
     ///
@@ -133,14 +135,31 @@
 
         Err(Error::new(
             ErrorKind::Unsupported,
             "operation is not supported",
         ))
     }
 
+    /// Invoke the `append` operation on the specified path, returns a
+    /// appended size if operate successful.
+    ///
+    ///  Require [`Capability::append`]
+    ///
+    /// # Behavior
+    ///
+    /// - Input path MUST be file path, DON'T NEED to check mode.
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        let (_, _) = (path, args);
+
+        Err(Error::new(
+            ErrorKind::Unsupported,
+            "operation is not supported",
+        ))
+    }
+
     /// Invoke the `copy` operation on the specified `from` path and `to` path.
     ///
     /// Require [Capability::copy]
     ///
     /// # Behaviour
     ///
     /// - `from` and `to` MUST be file path, DON'T NEED to check mode.
@@ -367,14 +386,15 @@
 /// Dummy implementation of accessor.
 #[async_trait]
 impl Accessor for () {
     type Reader = ();
     type BlockingReader = ();
     type Writer = ();
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         AccessorInfo {
             scheme: Scheme::Custom("dummy"),
             root: "".to_string(),
@@ -388,14 +408,15 @@
 /// `Accessor` for `Arc<dyn Accessor>`.
 #[async_trait]
 impl<T: Accessor + ?Sized> Accessor for Arc<T> {
     type Reader = T::Reader;
     type BlockingReader = T::BlockingReader;
     type Writer = T::Writer;
     type BlockingWriter = T::BlockingWriter;
+    type Appender = T::Appender;
     type Pager = T::Pager;
     type BlockingPager = T::BlockingPager;
 
     fn info(&self) -> AccessorInfo {
         self.as_ref().info()
     }
 
@@ -406,14 +427,18 @@
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         self.as_ref().read(path, args).await
     }
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         self.as_ref().write(path, args).await
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        self.as_ref().append(path, args).await
+    }
+
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         self.as_ref().copy(from, to, args).await
     }
 
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         self.as_ref().rename(from, to, args).await
     }
@@ -468,14 +493,15 @@
 /// FusedAccessor is the type erased accessor with `Arc<dyn Accessor>`.
 pub type FusedAccessor = Arc<
     dyn Accessor<
         Reader = oio::Reader,
         BlockingReader = oio::BlockingReader,
         Writer = oio::Writer,
         BlockingWriter = oio::BlockingWriter,
+        Appender = oio::Appender,
         Pager = oio::Pager,
         BlockingPager = oio::BlockingPager,
     >,
 >;
 
 /// Metadata for accessor, users can use this metadata to get information of underlying backend.
 #[derive(Clone, Debug, Default)]
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/api.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 #[async_trait]
 impl<S: Adapter> Accessor for Backend<S> {
     type Reader = oio::Cursor;
     type BlockingReader = oio::Cursor;
     type Writer = KvWriter<S>;
     type BlockingWriter = KvWriter<S>;
+    type Appender = ();
     type Pager = KvPager;
     type BlockingPager = KvPager;
 
     fn info(&self) -> AccessorInfo {
         let mut am: AccessorInfo = self.kv.metadata().into();
         am.set_root(&self.root);
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/api.rs`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::{fmt::Debug, mem::size_of};
+use std::fmt::Debug;
+use std::mem::size_of;
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use chrono::Utc;
 
 use crate::EntryMode;
 use crate::Error;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
 #[async_trait]
 impl<S: Adapter> Accessor for Backend<S> {
     type Reader = oio::Cursor;
     type BlockingReader = oio::Cursor;
     type Writer = KvWriter<S>;
     type BlockingWriter = KvWriter<S>;
+    type Appender = ();
     type Pager = KvPager;
     type BlockingPager = KvPager;
 
     fn info(&self) -> AccessorInfo {
         let kv_info = self.kv.info();
         let mut am: AccessorInfo = AccessorInfo::default();
         am.set_root(&self.root);
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/adapters/typed_kv/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/chrono_util.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/chrono_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/body.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/body.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_content_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/bytes_range.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/client.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/client.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/header.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/header.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/multipart.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/multipart.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/http_util/uri.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/http_util/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/layer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/layer.rs`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 /// #[async_trait]
 /// impl<A: Accessor> LayeredAccessor for TraceAccessor<A> {
 ///     type Inner = A;
 ///     type Reader = A::Reader;
 ///     type BlockingReader = A::BlockingReader;
 ///     type Writer = A::Writer;
 ///     type BlockingWriter = A::BlockingWriter;
+///     type Appender = A::Appender;
 ///     type Pager = A::Pager;
 ///     type BlockingPager = A::BlockingPager;
 ///
 ///     fn inner(&self) -> &Self::Inner {
 ///         &self.inner
 ///     }
 ///
@@ -90,14 +91,18 @@
 ///         &self,
 ///         path: &str,
 ///         args: OpWrite,
 ///     ) -> Result<(RpWrite, Self::BlockingWriter)> {
 ///         self.inner.blocking_write(path, args)
 ///     }
 ///
+///     async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+///         self.inner.append(path, args).await
+///     }
+///
 ///     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
 ///         self.inner.list(path, args).await
 ///     }
 ///
 ///     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
 ///         self.inner.blocking_list(path, args)
 ///     }
@@ -130,14 +135,15 @@
 #[async_trait]
 pub trait LayeredAccessor: Send + Sync + Debug + Unpin + 'static {
     type Inner: Accessor;
     type Reader: oio::Read;
     type BlockingReader: oio::BlockingRead;
     type Writer: oio::Write;
     type BlockingWriter: oio::BlockingWrite;
+    type Appender: oio::Append;
     type Pager: oio::Page;
     type BlockingPager: oio::BlockingPage;
 
     fn inner(&self) -> &Self::Inner;
 
     fn metadata(&self) -> AccessorInfo {
         self.inner().info()
@@ -147,14 +153,16 @@
         self.inner().create_dir(path, args).await
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)>;
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)>;
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)>;
+
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         self.inner().copy(from, to, args).await
     }
 
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         self.inner().rename(from, to, args).await
     }
@@ -206,14 +214,15 @@
 
 #[async_trait]
 impl<L: LayeredAccessor> Accessor for L {
     type Reader = L::Reader;
     type BlockingReader = L::BlockingReader;
     type Writer = L::Writer;
     type BlockingWriter = L::BlockingWriter;
+    type Appender = L::Appender;
     type Pager = L::Pager;
     type BlockingPager = L::BlockingPager;
 
     fn info(&self) -> AccessorInfo {
         (self as &L).metadata()
     }
 
@@ -225,14 +234,18 @@
         (self as &L).read(path, args).await
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         (self as &L).write(path, args).await
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        (self as &L).append(path, args).await
+    }
+
     async fn copy(&self, from: &str, to: &str, args: OpCopy) -> Result<RpCopy> {
         (self as &L).copy(from, to, args).await
     }
 
     async fn rename(&self, from: &str, to: &str, args: OpRename) -> Result<RpRename> {
         (self as &L).rename(from, to, args).await
     }
@@ -319,14 +332,15 @@
 
     #[async_trait::async_trait]
     impl<A: Accessor> Accessor for Test<A> {
         type Reader = ();
         type BlockingReader = ();
         type Writer = ();
         type BlockingWriter = ();
+        type Appender = ();
         type Pager = ();
         type BlockingPager = ();
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
             am.set_scheme(Scheme::Custom("test"));
             am
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/cursor.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/cursor.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/entry.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_blocking_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/by_range.rs`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,15 @@
 
     #[async_trait]
     impl Accessor for MockReadService {
         type Reader = MockReader;
         type BlockingReader = ();
         type Writer = ();
         type BlockingWriter = ();
+        type Appender = ();
         type Pager = ();
         type BlockingPager = ();
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
             am.set_capability(Capability {
                 read: true,
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/from_fd.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_reader/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/into_streamable.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 mod write;
 pub use write::BlockingWrite;
 pub use write::BlockingWriter;
 pub use write::Write;
 pub use write::WriteOperation;
 pub use write::Writer;
 
+mod append;
+pub use append::Append;
+pub use append::AppendOperation;
+pub use append::Appender;
+
 mod cursor;
 pub use cursor::Cursor;
 pub use cursor::VectorCursor;
 
 mod into_streamable;
 pub use into_streamable::into_streamable_reader;
 pub use into_streamable::IntoStreamableReader;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/page.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/page.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/read.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/read.rs`

 * *Files 1% similar despite different names*

```diff
@@ -342,24 +342,24 @@
     }
 
     fn next(&mut self) -> Option<Result<Bytes>> {
         (**self).next()
     }
 }
 
-impl std::io::Read for dyn BlockingRead {
+impl io::Read for dyn BlockingRead {
     #[inline]
     fn read(&mut self, buf: &mut [u8]) -> io::Result<usize> {
         let this: &mut dyn BlockingRead = &mut *self;
         this.read(buf)
             .map_err(|err| io::Error::new(io::ErrorKind::Interrupted, err))
     }
 }
 
-impl std::io::Seek for dyn BlockingRead {
+impl io::Seek for dyn BlockingRead {
     #[inline]
     fn seek(&mut self, pos: io::SeekFrom) -> io::Result<u64> {
         let this: &mut dyn BlockingRead = &mut *self;
         this.seek(pos)
             .map_err(|err| io::Error::new(io::ErrorKind::Interrupted, err))
     }
 }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_flat_pager.rs`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
 
     #[async_trait]
     impl Accessor for MockService {
         type Reader = ();
         type BlockingReader = ();
         type Writer = ();
         type BlockingWriter = ();
+        type Appender = ();
         type Pager = ();
         type BlockingPager = MockPager;
 
         fn info(&self) -> AccessorInfo {
             let mut am = AccessorInfo::default();
             am.capability_mut().list = true;
             am.capability_mut().list_with_delimiter_slash = true;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/to_hierarchy_pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/oio/write.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/oio/write.rs`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,17 @@
         Err(Error::new(
             ErrorKind::Unsupported,
             "output writer doesn't support close",
         ))
     }
 }
 
-/// `Box<dyn Write>` won't implement `Write` automatically. To make Writer
-/// work as expected, we must add this impl.
+/// `Box<dyn Write>` won't implement `Write` automatically.
+///
+/// To make Writer work as expected, we must add this impl.
 #[async_trait]
 impl<T: Write + ?Sized> Write for Box<T> {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         (**self).write(bs).await
     }
 
     async fn abort(&mut self) -> Result<()> {
@@ -164,14 +165,15 @@
             ErrorKind::Unsupported,
             "output writer doesn't support close",
         ))
     }
 }
 
 /// `Box<dyn BlockingWrite>` won't implement `BlockingWrite` automatically.
+///
 /// To make BlockingWriter work as expected, we must add this impl.
 impl<T: BlockingWrite + ?Sized> BlockingWrite for Box<T> {
     fn write(&mut self, bs: Bytes) -> Result<()> {
         (**self).write(bs)
     }
 
     fn close(&mut self) -> Result<()> {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/operation.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/operation.rs`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
     Info,
     /// Operation for [`crate::raw::Accessor::create_dir`]
     CreateDir,
     /// Operation for [`crate::raw::Accessor::read`]
     Read,
     /// Operation for [`crate::raw::Accessor::write`]
     Write,
+    /// Operation for [`crate::raw::Accessor::append`]
+    Append,
     /// Operation for [`crate::raw::Accessor::copy`]
     Copy,
     /// Operation for [`crate::raw::Accessor::rename`]
     Rename,
     /// Operation for [`crate::raw::Accessor::stat`]
     Stat,
     /// Operation for [`crate::raw::Accessor::delete`]
     Delete,
     /// Operation for [`crate::raw::Accessor::list`]
     List,
-    /// Operation for [`crate::raw::Accessor::scan`]
-    Scan,
     /// Operation for [`crate::raw::Accessor::batch`]
     Batch,
     /// Operation for [`crate::raw::Accessor::presign`]
     Presign,
     /// Operation for [`crate::raw::Accessor::blocking_create_dir`]
     BlockingCreateDir,
     /// Operation for [`crate::raw::Accessor::blocking_read`]
@@ -59,16 +59,14 @@
     BlockingRename,
     /// Operation for [`crate::raw::Accessor::blocking_stat`]
     BlockingStat,
     /// Operation for [`crate::raw::Accessor::blocking_delete`]
     BlockingDelete,
     /// Operation for [`crate::raw::Accessor::blocking_list`]
     BlockingList,
-    /// Operation for [`crate::raw::Accessor::blocking_scan`]
-    BlockingScan,
 }
 
 impl Operation {
     /// Convert self into static str.
     pub fn into_static(self) -> &'static str {
         self.into()
     }
@@ -83,31 +81,30 @@
 impl From<Operation> for &'static str {
     fn from(v: Operation) -> &'static str {
         match v {
             Operation::Info => "metadata",
             Operation::CreateDir => "create_dir",
             Operation::Read => "read",
             Operation::Write => "write",
+            Operation::Append => "append",
             Operation::Copy => "copy",
             Operation::Rename => "rename",
             Operation::Stat => "stat",
             Operation::Delete => "delete",
             Operation::List => "list",
-            Operation::Scan => "scan",
             Operation::Presign => "presign",
             Operation::Batch => "batch",
             Operation::BlockingCreateDir => "blocking_create_dir",
             Operation::BlockingRead => "blocking_read",
             Operation::BlockingWrite => "blocking_write",
             Operation::BlockingCopy => "blocking_copy",
             Operation::BlockingRename => "blocking_rename",
             Operation::BlockingStat => "blocking_stat",
             Operation::BlockingDelete => "blocking_delete",
             Operation::BlockingList => "blocking_list",
-            Operation::BlockingScan => "blocking_scan",
         }
     }
 }
 
 impl From<Operation> for String {
     fn from(v: Operation) -> Self {
         v.into_static().to_string()
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/path.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/path.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/rps.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/rps.rs`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,25 @@
 impl RpWrite {
     /// Create a new reply for `write`.
     pub fn new() -> Self {
         Self {}
     }
 }
 
+/// Reply for `append` operation.
+#[derive(Debug, Clone, Default)]
+pub struct RpAppend {}
+
+impl RpAppend {
+    /// Create a new reply for `append`.
+    pub fn new() -> Self {
+        Self {}
+    }
+}
+
 /// Reply for `copy` operation.
 #[derive(Debug, Clone, Default)]
 pub struct RpCopy {}
 
 impl RpCopy {
     /// Create a new reply for `copy`.
     pub fn new() -> Self {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/serde_util.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/serde_util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/raw/version.rs` & `opendal-0.35.0/local_dependencies/opendal/src/raw/version.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azblob/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -48,92 +48,15 @@
     "blob.core.chinacloudapi.cn",
 ];
 
 const AZBLOB_BATCH_LIMIT: usize = 256;
 
 /// Azure Storage Blob services support.
 ///
-/// # Capabilities
-///
-/// This service can be used to:
-///
-/// - [x] stat
-/// - [x] read
-/// - [x] write
-/// - [x] create_dir
-/// - [x] delete
-/// - [x] copy
-/// - [ ] rename
-/// - [x] list
-/// - [x] scan
-/// - [x] presign
-/// - [ ] blocking
-///
-/// # Configuration
-///
-/// - `root`: Set the work dir for backend.
-/// - `container`: Set the container name for backend.
-/// - `endpoint`: Set the endpoint for backend.
-/// - `account_name`: Set the account_name for backend.
-/// - `account_key`: Set the account_key for backend.
-///
-/// Refer to public API docs for more information.
-///
-/// # Example
-///
-/// This example works on [Azurite](https://github.com/Azure/Azurite) for local developments.
-///
-/// ## Start local blob service
-///
-/// ```shell
-/// docker run -p 10000:10000 mcr.microsoft.com/azure-storage/azurite
-/// az storage container create --name test --connection-string "DefaultEndpointsProtocol=http;AccountName=devstoreaccount1;AccountKey=Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==;BlobEndpoint=http://127.0.0.1:10000/devstoreaccount1;"
-/// ```
-///
-/// ## Init OpenDAL Operator
-///
-/// ### Via Builder
-///
-/// ```no_run
-/// use std::sync::Arc;
-///
-/// use anyhow::Result;
-/// use opendal::services::Azblob;
-/// use opendal::Operator;
-///
-/// #[tokio::main]
-/// async fn main() -> Result<()> {
-///     // Create azblob backend builder.
-///     let mut builder = Azblob::default();
-///     // Set the root for azblob, all operations will happen under this root.
-///     //
-///     // NOTE: the root must be absolute path.
-///     builder.root("/path/to/dir");
-///     // Set the container name, this is required.
-///     builder.container("test");
-///     // Set the endpoint, this is required.
-///     //
-///     // For examples:
-///     // - "http://127.0.0.1:10000/devstoreaccount1"
-///     // - "https://accountname.blob.core.windows.net"
-///     builder.endpoint("http://127.0.0.1:10000/devstoreaccount1");
-///     // Set the account_name and account_key.
-///     //
-///     // OpenDAL will try load credential from the env.
-///     // If credential not set and no valid credential in env, OpenDAL will
-///     // send request without signing like anonymous user.
-///     builder.account_name("devstoreaccount1");
-///     builder.account_key("Eby8vdM02xNOcqFlqUwJPLlmEtlCDXJ1OUzFT50uSRZ6IFsuFq2UVErCz4I6tq/K1SZFPTOtr/KBHBeksoGMGw==");
-///
-///     // `Accessor` provides the low level APIs, we will use `Operator` normally.
-///     let op: Operator = Operator::new(builder)?.finish();
-///
-///     Ok(())
-/// }
-/// ```
+#[doc = include_str!("docs.md")]
 #[derive(Default, Clone)]
 pub struct AzblobBuilder {
     root: Option<String>,
     container: String,
     endpoint: Option<String>,
     account_name: Option<String>,
     account_key: Option<String>,
@@ -384,14 +307,15 @@
         let config_loader = AzureStorageConfig {
             account_name: self
                 .account_name
                 .clone()
                 .or_else(|| infer_storage_name_from_endpoint(endpoint.as_str())),
             account_key: self.account_key.clone(),
             sas_token: self.sas_token.clone(),
+            ..Default::default()
         };
 
         let cred_loader = AzureStorageLoader::new(config_loader);
 
         let signer = AzureStorageSigner::new();
         let batch_signer = AzureStorageSigner::new().omit_service_version();
 
@@ -445,14 +369,15 @@
 
 #[async_trait]
 impl Accessor for AzblobBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = AzblobWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = AzblobPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azblob)
             .set_root(&self.core.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azblob/batch.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/batch.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azblob/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azblob/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azblob/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azblob/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azblob/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azblob/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -257,14 +257,15 @@
         let config_loader = AzureStorageConfig {
             account_name: self
                 .account_name
                 .clone()
                 .or_else(|| infer_storage_name_from_endpoint(endpoint.as_str())),
             account_key: self.account_key.clone(),
             sas_token: None,
+            ..Default::default()
         };
 
         let cred_loader = AzureStorageLoader::new(config_loader);
         let signer = AzureStorageSigner::new();
 
         debug!("backend build finished: {:?}", &self);
         Ok(AzdfsBackend {
@@ -300,14 +301,15 @@
 
 #[async_trait]
 impl Accessor for AzdfsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = AzdfsWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = AzdfsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Azdfs)
             .set_root(&self.core.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/azdfs/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/azdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/dashmap/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/dashmap/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/dashmap/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/fs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/fs/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,22 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::cmp::min;
 use std::collections::HashMap;
-use std::io;
 use std::io::SeekFrom;
 use std::path::Path;
 use std::path::PathBuf;
 
 use async_compat::Compat;
 use async_trait::async_trait;
 use chrono::DateTime;
 use log::debug;
-use tokio::fs;
 use uuid::Uuid;
 
 use super::error::parse_io_error;
 use super::pager::FsPager;
 use super::writer::FsWriter;
 use crate::ops::*;
 use crate::raw::*;
@@ -153,30 +151,30 @@
                 "root is not specified",
             )),
         }?;
         debug!("backend use root {}", root.to_string_lossy());
 
         // If root dir is not exist, we must create it.
         if let Err(e) = std::fs::metadata(&root) {
-            if e.kind() == io::ErrorKind::NotFound {
+            if e.kind() == std::io::ErrorKind::NotFound {
                 std::fs::create_dir_all(&root).map_err(|e| {
                     Error::new(ErrorKind::Unexpected, "create root dir failed")
                         .with_operation("Builder::build")
                         .with_context("root", root.to_string_lossy())
                         .set_source(e)
                 })?;
             }
         }
 
         let atomic_write_dir = self.atomic_write_dir.take();
 
         // If atomic write dir is not exist, we must create it.
         if let Some(d) = &atomic_write_dir {
             if let Err(e) = std::fs::metadata(d) {
-                if e.kind() == io::ErrorKind::NotFound {
+                if e.kind() == std::io::ErrorKind::NotFound {
                     std::fs::create_dir_all(d).map_err(|e| {
                         Error::new(ErrorKind::Unexpected, "create atomic write dir failed")
                             .with_operation("Builder::build")
                             .with_context("atomic_write_dir", d.to_string_lossy())
                             .set_source(e)
                     })?;
                 }
@@ -280,26 +278,29 @@
                     ErrorKind::Unexpected,
                     "path should have parent but not, it must be malformed",
                 )
                 .with_context("input", p.to_string_lossy())
             })?
             .to_path_buf();
 
-        fs::create_dir_all(&parent).await.map_err(parse_io_error)?;
+        tokio::fs::create_dir_all(&parent)
+            .await
+            .map_err(parse_io_error)?;
 
         Ok(p)
     }
 }
 
 #[async_trait]
 impl Accessor for FsBackend {
     type Reader = oio::into_reader::FdReader<Compat<tokio::fs::File>>;
     type BlockingReader = oio::into_blocking_reader::FdReader<std::fs::File>;
     type Writer = FsWriter<tokio::fs::File>;
     type BlockingWriter = FsWriter<std::fs::File>;
+    type Appender = ();
     type Pager = Option<FsPager<tokio::fs::ReadDir>>;
     type BlockingPager = Option<FsPager<std::fs::ReadDir>>;
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Fs)
             .set_root(&self.root.to_string_lossy())
@@ -327,15 +328,17 @@
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
         let p = self.root.join(path.trim_end_matches('/'));
 
-        fs::create_dir_all(&p).await.map_err(parse_io_error)?;
+        tokio::fs::create_dir_all(&p)
+            .await
+            .map_err(parse_io_error)?;
 
         Ok(RpCreateDir::default())
     }
 
     /// # Notes
     ///
     /// There are three ways to get the total file length:
@@ -346,15 +349,15 @@
     ///
     /// Benchmark could be found [here](https://gist.github.com/Xuanwo/48f9cfbc3022ea5f865388bb62e1a70f)
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
         use oio::ReadExt;
 
         let p = self.root.join(path.trim_end_matches('/'));
 
-        let mut f = fs::OpenOptions::new()
+        let mut f = tokio::fs::OpenOptions::new()
             .read(true)
             .open(&p)
             .await
             .map_err(parse_io_error)?;
 
         let total_length = if self.enable_path_check {
             // Get fs metadata of file at given path, ensuring it is not a false-positive due to slash normalization.
@@ -491,17 +494,17 @@
         let p = self.root.join(path.trim_end_matches('/'));
 
         let meta = tokio::fs::metadata(&p).await;
 
         match meta {
             Ok(meta) => {
                 if meta.is_dir() {
-                    fs::remove_dir(&p).await.map_err(parse_io_error)?;
+                    tokio::fs::remove_dir(&p).await.map_err(parse_io_error)?;
                 } else {
-                    fs::remove_file(&p).await.map_err(parse_io_error)?;
+                    tokio::fs::remove_file(&p).await.map_err(parse_io_error)?;
                 }
 
                 Ok(RpDelete::default())
             }
             Err(err) if err.kind() == std::io::ErrorKind::NotFound => Ok(RpDelete::default()),
             Err(err) => Err(parse_io_error(err)),
         }
@@ -509,15 +512,15 @@
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
         let p = self.root.join(path.trim_end_matches('/'));
 
         let f = match tokio::fs::read_dir(&p).await {
             Ok(rd) => rd,
             Err(e) => {
-                return if e.kind() == io::ErrorKind::NotFound {
+                return if e.kind() == std::io::ErrorKind::NotFound {
                     Ok((RpList::default(), None))
                 } else {
                     Err(parse_io_error(e))
                 };
             }
         };
 
@@ -694,15 +697,15 @@
 
     fn blocking_list(&self, path: &str, args: OpList) -> Result<(RpList, Self::BlockingPager)> {
         let p = self.root.join(path.trim_end_matches('/'));
 
         let f = match std::fs::read_dir(p) {
             Ok(rd) => rd,
             Err(e) => {
-                return if e.kind() == io::ErrorKind::NotFound {
+                return if e.kind() == std::io::ErrorKind::NotFound {
                     Ok((RpList::default(), None))
                 } else {
                     Err(parse_io_error(e))
                 };
             }
         };
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/fs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/fs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/fs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/fs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/fs/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/fs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/fs/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/fs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ftp/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -310,14 +310,15 @@
 
 #[async_trait]
 impl Accessor for FtpBackend {
     type Reader = FtpReader;
     type BlockingReader = ();
     type Writer = FtpWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = FtpPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ftp)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ftp/err.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/err.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ftp/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ftp/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ftp/util.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/util.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ftp/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ftp/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gcs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -392,14 +392,15 @@
 
 #[async_trait]
 impl Accessor for GcsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = GcsWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = GcsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Gcs)
             .set_root(&self.core.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gcs/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gcs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gcs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gcs/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gcs/uri.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/uri.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gcs/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gcs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/obs/core.rs`

 * *Files 20% similar despite different names*

```diff
@@ -11,242 +11,283 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use async_trait::async_trait;
-use http::{header, Request, Response, StatusCode};
-use serde::Deserialize;
 use std::fmt::Debug;
+use std::fmt::Formatter;
+use std::time::Duration;
 
-use crate::{
-    ops::{OpDelete, OpRead, OpWrite},
-    raw::{
-        build_rooted_abs_path, new_request_build_error, parse_into_metadata, Accessor,
-        AccessorInfo, AsyncBody, HttpClient, IncomingAsyncBody, RpDelete, RpRead, RpWrite,
-    },
-    types::Result,
-    Capability, Error, ErrorKind,
-};
-
-use super::{error::parse_error, writer::GdriveWriter};
-
-#[derive(Clone)]
-pub struct GdriveBackend {
-    root: String,
-    access_token: String,
-    client: HttpClient,
+use http::header::CACHE_CONTROL;
+use http::header::CONTENT_LENGTH;
+use http::header::CONTENT_TYPE;
+use http::header::IF_MATCH;
+use http::header::IF_NONE_MATCH;
+use http::Request;
+use http::Response;
+use reqsign::HuaweicloudObsCredential;
+use reqsign::HuaweicloudObsCredentialLoader;
+use reqsign::HuaweicloudObsSigner;
+
+use crate::raw::*;
+use crate::*;
+
+pub struct ObsCore {
+    pub bucket: String,
+    pub root: String,
+    pub endpoint: String,
+
+    pub signer: HuaweicloudObsSigner,
+    pub loader: HuaweicloudObsCredentialLoader,
+    pub client: HttpClient,
 }
 
-impl GdriveBackend {
-    pub(crate) fn new(root: String, access_token: String, http_client: HttpClient) -> Self {
-        GdriveBackend {
-            root,
-            access_token,
-            client: http_client,
-        }
+impl Debug for ObsCore {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        f.debug_struct("Backend")
+            .field("root", &self.root)
+            .field("bucket", &self.bucket)
+            .field("endpoint", &self.endpoint)
+            .finish_non_exhaustive()
     }
 }
 
-impl Debug for GdriveBackend {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let mut de = f.debug_struct("GoolgeDriveBackend");
-        de.field("root", &self.root);
-        de.finish()
+impl ObsCore {
+    async fn load_credential(&self) -> Result<Option<HuaweicloudObsCredential>> {
+        let cred = self
+            .loader
+            .load()
+            .await
+            .map_err(new_request_credential_error)?;
+
+        if let Some(cred) = cred {
+            Ok(Some(cred))
+        } else {
+            Ok(None)
+        }
+    }
+
+    pub async fn sign<T>(&self, req: &mut Request<T>) -> Result<()> {
+        let cred = if let Some(cred) = self.load_credential().await? {
+            cred
+        } else {
+            return Ok(());
+        };
+
+        self.signer.sign(req, &cred).map_err(new_request_sign_error)
+    }
+
+    pub async fn sign_query<T>(&self, req: &mut Request<T>, duration: Duration) -> Result<()> {
+        let cred = if let Some(cred) = self.load_credential().await? {
+            cred
+        } else {
+            return Ok(());
+        };
+
+        self.signer
+            .sign_query(req, duration, &cred)
+            .map_err(new_request_sign_error)
+    }
+
+    #[inline]
+    pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
+        self.client.send(req).await
     }
 }
 
-#[async_trait]
-impl Accessor for GdriveBackend {
-    type Reader = IncomingAsyncBody;
-    type BlockingReader = ();
-    type Writer = GdriveWriter;
-    type BlockingWriter = ();
-    type Pager = ();
-    type BlockingPager = ();
+impl ObsCore {
+    pub async fn obs_get_object(
+        &self,
+        path: &str,
+        range: BytesRange,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.obs_get_object_request(path, range, if_match, if_none_match)?;
 
-    fn info(&self) -> AccessorInfo {
-        let mut ma = AccessorInfo::default();
-        ma.set_scheme(crate::Scheme::Gdrive)
-            .set_root(&self.root)
-            .set_capability(Capability {
-                read: true,
-                write: true,
-                delete: true,
-                ..Default::default()
-            });
+        self.sign(&mut req).await?;
 
-        ma
+        self.send(req).await
     }
 
-    async fn read(&self, path: &str, _args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.gdrive_get(path).await?;
+    pub fn obs_get_object_request(
+        &self,
+        path: &str,
+        range: BytesRange,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+
+        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
-        let status = resp.status();
+        let mut req = Request::get(&url);
 
-        match status {
-            StatusCode::OK => {
-                let meta = parse_into_metadata(path, resp.headers())?;
-                Ok((RpRead::with_metadata(meta), resp.into_body()))
-            }
-            _ => Err(parse_error(resp).await?),
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
+
+        if !range.is_full() {
+            req = req.header(http::header::RANGE, range.to_header())
         }
-    }
 
-    async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.content_length().is_none() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "write without content length is not supported",
-            ));
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
-        Ok((
-            RpWrite::default(),
-            GdriveWriter::new(self.clone(), args, String::from(path)),
-        ))
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        Ok(req)
     }
 
-    async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let resp = self.gdrive_delete(path).await?;
+    pub fn obs_put_object_request(
+        &self,
+        path: &str,
+        size: Option<usize>,
+        content_type: Option<&str>,
+        cache_control: Option<&str>,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
 
-        let status = resp.status();
+        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
+
+        let mut req = Request::put(&url);
+
+        if let Some(size) = size {
+            req = req.header(CONTENT_LENGTH, size)
+        }
+        if let Some(cache_control) = cache_control {
+            req = req.header(CACHE_CONTROL, cache_control)
+        }
 
-        match status {
-            StatusCode::NO_CONTENT => Ok(RpDelete::default()),
-            _ => Err(parse_error(resp).await?),
+        if let Some(mime) = content_type {
+            req = req.header(CONTENT_TYPE, mime)
         }
+
+        let req = req.body(body).map_err(new_request_build_error)?;
+
+        Ok(req)
     }
-}
 
-impl GdriveBackend {
-    async fn get_abs_root_id(&self) -> String {
-        let mut req = Request::get("https://www.googleapis.com/drive/v3/files/root");
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
-        let req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)
-            .unwrap();
+    pub async fn obs_head_object(
+        &self,
+        path: &str,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.obs_head_object_request(path, if_match, if_none_match)?;
 
-        let resp = self.client.send(req).await.unwrap();
+        self.sign(&mut req).await?;
 
-        let body_value: GdriveFile =
-            serde_json::from_slice(&resp.into_body().bytes().await.unwrap()).unwrap();
-        let root_id = String::from(body_value.id.as_str());
-        root_id
+        self.send(req).await
     }
 
-    async fn get_file_id_by_path(&self, file_path: &str) -> String {
-        let path = build_rooted_abs_path(&self.root, file_path);
-        let auth_header_content = format!("Bearer {}", self.access_token);
+    pub fn obs_head_object_request(
+        &self,
+        path: &str,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
 
-        let mut parent_id = self.get_abs_root_id().await;
-        let file_path_items: Vec<&str> = path.split('/').filter(|&x| !x.is_empty()).collect();
+        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
-        for (i, item) in file_path_items.iter().enumerate() {
-            let mut query = format!(
-                "name = '{}' and parents = '{}' and trashed = false",
-                item, parent_id
-            );
-            if i != file_path_items.len() - 1 {
-                query += "and mimeType = 'application/vnd.google-apps.folder'";
-            }
-            let query: String = query.chars().filter(|c| !c.is_whitespace()).collect();
+        // The header 'Origin' is optional for API calling, the doc has mistake, confirmed with customer service of huaweicloud.
+        // https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0084.html
 
-            let mut req = Request::get(format!(
-                "https://www.googleapis.com/drive/v3/files?q={}",
-                query
-            ));
-            req = req.header(header::AUTHORIZATION, &auth_header_content);
-            let req = req
-                .body(AsyncBody::default())
-                .map_err(new_request_build_error)
-                .unwrap();
+        let mut req = Request::head(&url);
 
-            let resp = self.client.send(req).await.unwrap();
+        if let Some(if_match) = if_match {
+            req = req.header(IF_MATCH, if_match);
+        }
 
-            let body_value: GdriveFileList =
-                serde_json::from_slice(&resp.into_body().bytes().await.unwrap()).unwrap();
-            parent_id = String::from(body_value.files[0].id.as_str());
+        if let Some(if_none_match) = if_none_match {
+            req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
-        parent_id
+        let req = req
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
+
+        Ok(req)
     }
 
-    async fn gdrive_get(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let url: String = format!(
-            "https://www.googleapis.com/drive/v3/files/{}?alt=media",
-            self.get_file_id_by_path(path).await
-        );
+    pub async fn obs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
 
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        let mut req = Request::get(&url);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
+        let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
-        let req = req
+        let req = Request::delete(&url);
+
+        let mut req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send(req).await
+        self.sign(&mut req).await?;
+
+        self.send(req).await
     }
 
-    pub async fn gdrive_update(
+    pub async fn obs_copy_object(
         &self,
-        path: &str,
-        size: Option<usize>,
-        content_type: Option<&str>,
-        body: AsyncBody,
+        from: &str,
+        to: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let url = format!(
-            "https://www.googleapis.com/upload/drive/v3/files/{}",
-            self.get_file_id_by_path(path).await
-        );
-
-        let mut req = Request::patch(&url);
-
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
+        let source = build_abs_path(&self.root, from);
+        let target = build_abs_path(&self.root, to);
 
-        if let Some(size) = size {
-            req = req.header(header::CONTENT_LENGTH, size)
-        }
+        let source = format!("/{}/{}", self.bucket, percent_encode_path(&source));
+        let url = format!("{}/{}", self.endpoint, percent_encode_path(&target));
 
-        if let Some(mime) = content_type {
-            req = req.header(header::CONTENT_TYPE, mime)
-        }
+        let mut req = Request::put(&url)
+            .header("x-obs-copy-source", percent_encode_path(&source))
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
-        let req = req.body(body).map_err(new_request_build_error)?;
+        self.sign(&mut req).await?;
 
-        self.client.send(req).await
+        self.send(req).await
     }
 
-    async fn gdrive_delete(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let url = format!(
-            "https://www.googleapis.com/drive/v3/files/{}",
-            self.get_file_id_by_path(path).await
-        );
+    pub async fn obs_list_objects(
+        &self,
+        path: &str,
+        next_marker: &str,
+        delimiter: &str,
+        limit: Option<usize>,
+    ) -> Result<Response<IncomingAsyncBody>> {
+        let p = build_abs_path(&self.root, path);
 
-        let mut req = Request::delete(&url);
+        let mut queries = vec![];
+        if !path.is_empty() {
+            queries.push(format!("prefix={}", percent_encode_path(&p)));
+        }
+        if !delimiter.is_empty() {
+            queries.push(format!("delimiter={delimiter}"));
+        }
+        if let Some(limit) = limit {
+            queries.push(format!("max-keys={limit}"));
+        }
+        if !next_marker.is_empty() {
+            queries.push(format!("marker={next_marker}"));
+        }
 
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
+        let url = if queries.is_empty() {
+            self.endpoint.to_string()
+        } else {
+            format!("{}?{}", self.endpoint, queries.join("&"))
+        };
 
-        let req = req
+        let mut req = Request::get(&url)
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.client.send(req).await
-    }
-}
-
-#[derive(Deserialize)]
-struct GdriveFile {
-    id: String,
-}
+        self.sign(&mut req).await?;
 
-#[derive(Deserialize)]
-struct GdriveFileList {
-    files: Vec<GdriveFile>,
+        self.send(req).await
+    }
 }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/builder.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/builder.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
-use std::fmt::{Debug, Formatter};
+use std::fmt::Debug;
+use std::fmt::Formatter;
 
 use log::debug;
 
 use super::backend::GdriveBackend;
-use crate::raw::{normalize_root, HttpClient};
+use crate::raw::normalize_root;
+use crate::raw::HttpClient;
 use crate::Scheme;
 use crate::*;
 
 /// [GoogleDrive](https://drive.google.com/) backend support.
 ///
 /// # Capabilities
 ///
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/redis/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,12 +12,8 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-mod builder;
-mod error;
-
-pub use builder::GdriveBuilder as Gdrive;
-mod writer;
+pub use backend::RedisBuilder as Redis;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/gdrive/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/writer.rs`

 * *Files 7% similar despite different names*

```diff
@@ -11,42 +11,43 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::GdriveBackend;
+use super::core::GdriveCore;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 pub struct GdriveWriter {
-    backend: GdriveBackend,
-
+    core: Arc<GdriveCore>,
     op: OpWrite,
     path: String,
 }
 
 impl GdriveWriter {
-    pub fn new(backend: GdriveBackend, op: OpWrite, path: String) -> Self {
-        GdriveWriter { backend, op, path }
+    pub fn new(core: Arc<GdriveCore>, op: OpWrite, path: String) -> Self {
+        GdriveWriter { core, op, path }
     }
 }
 
 #[async_trait]
 impl oio::Write for GdriveWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let resp = self
-            .backend
+            .core
             .gdrive_update(
                 &self.path,
                 Some(bs.len()),
                 self.op.content_type(),
                 AsyncBody::Bytes(bs),
             )
             .await?;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ghac/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/backend.rs`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,15 @@
 
 #[async_trait]
 impl Accessor for GhacBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = GhacWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ghac)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ghac/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ghac/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ghac/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ghac/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 /// - [x] delete
 /// - [ ] copy
 /// - [ ] rename
 /// - [x] list
 /// - [ ] ~~scan~~
 /// - [ ] ~~presign~~
 /// - [x] blocking
+///
 /// # Differences with webhdfs
 ///
 /// [Webhdfs][crate::services::Webhdfs] is powered by hdfs's RESTful HTTP API.
 ///
 /// # Features
 ///
 /// HDFS support needs to enable feature `services-hdfs`.
@@ -230,14 +231,15 @@
 
 #[async_trait]
 impl Accessor for HdfsBackend {
     type Reader = oio::into_reader::FdReader<hdrs::AsyncFile>;
     type BlockingReader = oio::into_blocking_reader::FdReader<hdrs::File>;
     type Writer = HdfsWriter<hdrs::AsyncFile>;
     type BlockingWriter = HdfsWriter<hdrs::File>;
+    type Appender = ();
     type Pager = Option<HdfsPager>;
     type BlockingPager = Option<HdfsPager>;
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Hdfs)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/hdfs/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/hdfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/http/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/http/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,15 @@
 
 #[async_trait]
 impl Accessor for HttpBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = ();
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Http)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/http/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/http/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/http/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/http/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -213,14 +213,15 @@
 
 #[async_trait]
 impl Accessor for IpfsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = ();
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = DirStream;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Ipfs)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/ipld.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/ipld.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipfs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 /// - [x] delete
 /// - [ ] copy
 /// - [ ] rename
 /// - [x] list
 /// - [ ] scan
 /// - [ ] presign
 /// - [ ] blocking
-///
 #[derive(Clone)]
 pub struct IpmfsBackend {
     root: String,
     endpoint: String,
     client: HttpClient,
 }
 
@@ -80,14 +79,15 @@
 
 #[async_trait]
 impl Accessor for IpmfsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = IpmfsWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = IpmfsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Ipmfs)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/builder.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/ipmfs/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/ipmfs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/memcached/ascii.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/memcached/ascii.rs`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use crate::*;
-
-use super::backend::parse_io_error;
 use tokio::io::AsyncBufReadExt;
 use tokio::io::AsyncReadExt;
 use tokio::io::AsyncWriteExt;
 use tokio::io::BufReader;
 use tokio::net::TcpStream;
 
+use super::backend::parse_io_error;
+use crate::*;
+
 pub struct Connection {
     io: BufReader<TcpStream>,
     buf: Vec<u8>,
 }
 
 impl Connection {
     pub fn new(io: TcpStream) -> Self {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/memcached/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/memcached/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/memcached/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/memcached/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/memory/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/memory/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/memory/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/memory/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 pub use azblob::Azblob;
 
 #[cfg(feature = "services-azdfs")]
 mod azdfs;
 #[cfg(feature = "services-azdfs")]
 pub use azdfs::Azdfs;
 
+#[cfg(feature = "services-cos")]
+mod cos;
+#[cfg(feature = "services-cos")]
+pub use cos::Cos;
+
 #[cfg(feature = "services-dashmap")]
 mod dashmap;
 #[cfg(feature = "services-dashmap")]
 pub use self::dashmap::Dashmap;
 
 #[cfg(feature = "services-fs")]
 mod fs;
@@ -147,15 +152,14 @@
 #[cfg(feature = "services-onedrive")]
 pub use onedrive::Onedrive;
 
 #[cfg(feature = "services-gdrive")]
 mod gdrive;
 #[cfg(feature = "services-gdrive")]
 pub use gdrive::Gdrive;
-
 #[cfg(feature = "services-webhdfs")]
 pub use webhdfs::Webhdfs;
 
 #[cfg(feature = "services-vercel-artifacts")]
 mod vercel_artifacts;
 #[cfg(feature = "services-vercel-artifacts")]
 pub use vercel_artifacts::VercelArtifacts;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/moka/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/moka/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/moka/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/moka/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/obs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/obs/backend.rs`

 * *Files 9% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 /// - [x] write
 /// - [x] create_dir
 /// - [x] delete
 /// - [x] copy
 /// - [ ] rename
 /// - [x] list
 /// - [x] scan
-/// - [ ] presign
+/// - [x] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
 /// - `root`: Set the work directory for backend
 /// - `bucket`: Set the container name for backend
 /// - `endpoint`: Customizable endpoint setting
@@ -297,14 +297,15 @@
 
 #[async_trait]
 impl Accessor for ObsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = ObsWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = ObsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Obs)
             .set_root(&self.core.root)
@@ -328,20 +329,57 @@
                 create_dir: true,
                 copy: true,
 
                 list: true,
                 list_with_delimiter_slash: true,
                 list_without_delimiter: true,
 
+                presign: true,
+                presign_stat: true,
+                presign_read: true,
+                presign_write: true,
+
                 ..Default::default()
             });
 
         am
     }
 
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        let mut req = match args.operation() {
+            PresignOperation::Stat(v) => {
+                self.core
+                    .obs_head_object_request(path, v.if_match(), v.if_none_match())?
+            }
+            PresignOperation::Read(v) => self.core.obs_get_object_request(
+                path,
+                v.range(),
+                v.if_match(),
+                v.if_none_match(),
+            )?,
+            PresignOperation::Write(v) => self.core.obs_put_object_request(
+                path,
+                None,
+                v.content_type(),
+                v.cache_control(),
+                AsyncBody::Empty,
+            )?,
+        };
+        self.core.sign_query(&mut req, args.expire()).await?;
+
+        // We don't need this request anymore, consume it directly.
+        let (parts, _) = req.into_parts();
+
+        Ok(RpPresign::new(PresignedRequest::new(
+            parts.method,
+            parts.uri,
+            parts.headers,
+        )))
+    }
+
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
         let mut req =
             self.core
                 .obs_put_object_request(path, Some(0), None, None, AsyncBody::Empty)?;
 
         self.core.sign(&mut req).await?;
 
@@ -407,15 +445,15 @@
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
         let resp = self
             .core
-            .obs_get_head_object(path, args.if_match(), args.if_none_match())
+            .obs_head_object(path, args.if_match(), args.if_none_match())
             .await?;
 
         let status = resp.status();
 
         // The response is very similar to azblob.
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/obs/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/cos/core.rs`

 * *Files 16% similar despite different names*

```diff
@@ -13,51 +13,52 @@
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::fmt::Debug;
 use std::fmt::Formatter;
+use std::time::Duration;
 
 use http::header::CACHE_CONTROL;
 use http::header::CONTENT_LENGTH;
 use http::header::CONTENT_TYPE;
 use http::header::IF_MATCH;
 use http::header::IF_NONE_MATCH;
 use http::Request;
 use http::Response;
-use reqsign::HuaweicloudObsCredential;
-use reqsign::HuaweicloudObsCredentialLoader;
-use reqsign::HuaweicloudObsSigner;
+use reqsign::TencentCosCredential;
+use reqsign::TencentCosCredentialLoader;
+use reqsign::TencentCosSigner;
 
 use crate::raw::*;
 use crate::*;
 
-pub struct ObsCore {
+pub struct CosCore {
     pub bucket: String,
     pub root: String,
     pub endpoint: String,
 
-    pub signer: HuaweicloudObsSigner,
-    pub loader: HuaweicloudObsCredentialLoader,
+    pub signer: TencentCosSigner,
+    pub loader: TencentCosCredentialLoader,
     pub client: HttpClient,
 }
 
-impl Debug for ObsCore {
+impl Debug for CosCore {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Backend")
             .field("root", &self.root)
             .field("bucket", &self.bucket)
             .field("endpoint", &self.endpoint)
             .finish_non_exhaustive()
     }
 }
 
-impl ObsCore {
-    async fn load_credential(&self) -> Result<Option<HuaweicloudObsCredential>> {
+impl CosCore {
+    async fn load_credential(&self) -> Result<Option<TencentCosCredential>> {
         let cred = self
             .loader
             .load()
             .await
             .map_err(new_request_credential_error)?;
 
         if let Some(cred) = cred {
@@ -73,28 +74,54 @@
         } else {
             return Ok(());
         };
 
         self.signer.sign(req, &cred).map_err(new_request_sign_error)
     }
 
+    pub async fn sign_query<T>(&self, req: &mut Request<T>, duration: Duration) -> Result<()> {
+        let cred = if let Some(cred) = self.load_credential().await? {
+            cred
+        } else {
+            return Ok(());
+        };
+
+        self.signer
+            .sign_query(req, duration, &cred)
+            .map_err(new_request_sign_error)
+    }
+
     #[inline]
     pub async fn send(&self, req: Request<AsyncBody>) -> Result<Response<IncomingAsyncBody>> {
         self.client.send(req).await
     }
 }
 
-impl ObsCore {
-    pub async fn obs_get_object(
+impl CosCore {
+    pub async fn cos_get_object(
         &self,
         path: &str,
         range: BytesRange,
         if_match: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.cos_get_object_request(path, range, if_match, if_none_match)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub fn cos_get_object_request(
+        &self,
+        path: &str,
+        range: BytesRange,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::get(&url);
 
         if let Some(if_match) = if_match {
@@ -105,24 +132,22 @@
             req = req.header(http::header::RANGE, range.to_header())
         }
 
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
-        let mut req = req
+        let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.sign(&mut req).await?;
-
-        self.send(req).await
+        Ok(req)
     }
 
-    pub fn obs_put_object_request(
+    pub fn cos_put_object_request(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         cache_control: Option<&str>,
         body: AsyncBody,
     ) -> Result<Request<AsyncBody>> {
@@ -144,47 +169,55 @@
         }
 
         let req = req.body(body).map_err(new_request_build_error)?;
 
         Ok(req)
     }
 
-    pub async fn obs_get_head_object(
+    pub async fn cos_head_object(
         &self,
         path: &str,
         if_match: Option<&str>,
         if_none_match: Option<&str>,
     ) -> Result<Response<IncomingAsyncBody>> {
+        let mut req = self.cos_head_object_request(path, if_match, if_none_match)?;
+
+        self.sign(&mut req).await?;
+
+        self.send(req).await
+    }
+
+    pub fn cos_head_object_request(
+        &self,
+        path: &str,
+        if_match: Option<&str>,
+        if_none_match: Option<&str>,
+    ) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
-        // The header 'Origin' is optional for API calling, the doc has mistake, confirmed with customer service of huaweicloud.
-        // https://support.huaweicloud.com/intl/en-us/api-obs/obs_04_0084.html
-
         let mut req = Request::head(&url);
 
         if let Some(if_match) = if_match {
             req = req.header(IF_MATCH, if_match);
         }
 
         if let Some(if_none_match) = if_none_match {
             req = req.header(IF_NONE_MATCH, if_none_match);
         }
 
-        let mut req = req
+        let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
-        self.sign(&mut req).await?;
-
-        self.send(req).await
+        Ok(req)
     }
 
-    pub async fn obs_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+    pub async fn cos_delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let req = Request::delete(&url);
 
         let mut req = req
@@ -192,36 +225,36 @@
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn obs_copy_object(
+    pub async fn cos_copy_object(
         &self,
         from: &str,
         to: &str,
     ) -> Result<Response<IncomingAsyncBody>> {
         let source = build_abs_path(&self.root, from);
         let target = build_abs_path(&self.root, to);
 
         let source = format!("/{}/{}", self.bucket, percent_encode_path(&source));
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&target));
 
         let mut req = Request::put(&url)
-            .header("x-obs-copy-source", percent_encode_path(&source))
+            .header("x-cos-copy-source", percent_encode_path(&source))
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
-    pub async fn obs_list_objects(
+    pub async fn cos_list_objects(
         &self,
         path: &str,
         next_marker: &str,
         delimiter: &str,
         limit: Option<usize>,
     ) -> Result<Response<IncomingAsyncBody>> {
         let p = build_abs_path(&self.root, path);
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/obs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/obs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/obs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/obs/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/obs/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/obs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/obs/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/obs/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/core.rs`

 * *Files 22% similar despite different names*

```diff
@@ -11,202 +11,208 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::collections::HashMap;
 use std::fmt::Debug;
+use std::fmt::Formatter;
+use std::sync::Arc;
 
-use async_trait::async_trait;
 use http::header;
+use http::request::Builder;
 use http::Request;
 use http::Response;
 use http::StatusCode;
+use serde::Deserialize;
+use tokio::sync::Mutex;
 
 use super::error::parse_error;
-use super::writer::OneDriveWriter;
-use crate::ops::OpRead;
-use crate::ops::OpWrite;
 use crate::raw::build_rooted_abs_path;
+use crate::raw::new_json_deserialize_error;
 use crate::raw::new_request_build_error;
-use crate::raw::parse_into_metadata;
-use crate::raw::parse_location;
 use crate::raw::percent_encode_path;
-use crate::raw::Accessor;
-use crate::raw::AccessorInfo;
 use crate::raw::AsyncBody;
 use crate::raw::HttpClient;
 use crate::raw::IncomingAsyncBody;
-use crate::raw::RpRead;
-use crate::raw::RpWrite;
 use crate::types::Result;
-use crate::Capability;
 use crate::Error;
 use crate::ErrorKind;
 
-#[derive(Clone)]
-pub struct OnedriveBackend {
-    root: String,
-    access_token: String,
-    client: HttpClient,
+pub struct GdriveCore {
+    pub root: String,
+    pub access_token: String,
+    pub client: HttpClient,
+    pub path_cache: Arc<Mutex<HashMap<String, String>>>,
 }
 
-impl OnedriveBackend {
-    pub(crate) fn new(root: String, access_token: String, http_client: HttpClient) -> Self {
-        Self {
-            root,
-            access_token,
-            client: http_client,
-        }
-    }
-}
-
-impl Debug for OnedriveBackend {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        let mut de = f.debug_struct("OneDriveBackend");
+impl Debug for GdriveCore {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        let mut de = f.debug_struct("GdriveCore");
         de.field("root", &self.root);
-        de.field("access_token", &self.access_token);
         de.finish()
     }
 }
 
-#[async_trait]
-impl Accessor for OnedriveBackend {
-    type Reader = IncomingAsyncBody;
-    type BlockingReader = ();
-    type Writer = OneDriveWriter;
-    type BlockingWriter = ();
-    type Pager = ();
-    type BlockingPager = ();
-
-    fn info(&self) -> AccessorInfo {
-        let mut ma = AccessorInfo::default();
-        ma.set_scheme(crate::Scheme::Onedrive)
-            .set_root(&self.root)
-            .set_capability(Capability {
-                read: true,
-                read_can_next: true,
-                write: true,
-                list: true,
-                copy: true,
-                rename: true,
-                ..Default::default()
-            });
+impl GdriveCore {
+    async fn get_abs_root_id(&self) -> Result<String> {
+        let root = "root";
 
-        ma
-    }
+        if let Some(root_id) = self.path_cache.lock().await.get(root) {
+            return Ok(root_id.to_string());
+        }
 
-    async fn read(&self, path: &str, _args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let resp = self.onedrive_get(path).await?;
+        let req = self
+            .sign(Request::get(
+                "https://www.googleapis.com/drive/v3/files/root",
+            ))
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
+        let resp = self.client.send(req).await?;
         let status = resp.status();
 
-        if status.is_redirection() {
-            let headers = resp.headers();
-            let location = parse_location(headers)?;
-
-            match location {
-                None => {
-                    return Err(Error::new(
-                        ErrorKind::ContentIncomplete,
-                        "redirect location not found in response",
-                    ));
-                }
-                Some(location) => {
-                    let resp = self.onedrive_get_redirection(location).await?;
-                    let meta = parse_into_metadata(path, resp.headers())?;
-                    Ok((RpRead::with_metadata(meta), resp.into_body()))
-                }
-            }
-        } else {
-            match status {
-                StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
-                    let meta = parse_into_metadata(path, resp.headers())?;
-                    Ok((RpRead::with_metadata(meta), resp.into_body()))
-                }
+        match status {
+            StatusCode::OK => {
+                let resp_body = &resp.into_body().bytes().await?;
+
+                let gdrive_file: GdriveFile =
+                    serde_json::from_slice(resp_body).map_err(new_json_deserialize_error)?;
+
+                let root_id = gdrive_file.id;
+
+                let mut cache_guard = self.path_cache.lock().await;
+                cache_guard.insert(root.to_owned(), root_id.clone());
 
-                _ => Err(parse_error(resp).await?),
+                Ok(root_id)
             }
+            _ => Err(parse_error(resp).await?),
         }
     }
 
-    async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
-        if args.content_length().is_none() {
-            return Err(Error::new(
-                ErrorKind::Unsupported,
-                "write without content length is not supported",
-            ));
+    async fn get_file_id_by_path(&self, file_path: &str) -> Result<String> {
+        let path = build_rooted_abs_path(&self.root, file_path);
+
+        if let Some(file_id) = self.path_cache.lock().await.get(&path) {
+            return Ok(file_id.to_string());
         }
 
-        let path = build_rooted_abs_path(&self.root, path);
-
-        Ok((
-            RpWrite::default(),
-            OneDriveWriter::new(self.clone(), args, path),
-        ))
-    }
-}
+        let mut parent_id = self.get_abs_root_id().await?;
+        let file_path_items: Vec<&str> = path.split('/').filter(|&x| !x.is_empty()).collect();
 
-impl OnedriveBackend {
-    async fn onedrive_get(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
-        let path = build_rooted_abs_path(&self.root, path);
-        let url: String = format!(
-            "https://graph.microsoft.com/v1.0/me/drive/root:{}:/content",
-            percent_encode_path(&path),
-        );
+        for (i, item) in file_path_items.iter().enumerate() {
+            let mut query = format!(
+                "name = '{}' and parents = '{}' and trashed = false",
+                item, parent_id
+            );
+            if i != file_path_items.len() - 1 {
+                query += "and mimeType = 'application/vnd.google-apps.folder'";
+            }
 
-        let mut req = Request::get(&url);
+            let req = self
+                .sign(Request::get(format!(
+                    "https://www.googleapis.com/drive/v3/files?q={}",
+                    percent_encode_path(&query)
+                )))
+                .body(AsyncBody::default())
+                .map_err(new_request_build_error)?;
+
+            let resp = self.client.send(req).await?;
+            let status = resp.status();
 
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
+            if status == StatusCode::OK {
+                let resp_body = &resp.into_body().bytes().await?;
 
-        let req = req
-            .body(AsyncBody::Empty)
-            .map_err(new_request_build_error)?;
+                let gdrive_file_list: GdriveFileList =
+                    serde_json::from_slice(resp_body).map_err(new_json_deserialize_error)?;
 
-        self.client.send(req).await
-    }
+                if gdrive_file_list.files.len() != 1 {
+                    return Err(Error::new(ErrorKind::Unexpected, &format!("Please ensure that the file corresponding to the path exists and is unique. The response body is {}", String::from_utf8_lossy(resp_body))));
+                }
 
-    async fn onedrive_get_redirection(&self, url: &str) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = Request::get(url);
+                parent_id = gdrive_file_list.files[0].id.clone();
+            } else {
+                return Err(parse_error(resp).await?);
+            }
+        }
 
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
+        let mut cache_guard = self.path_cache.lock().await;
+        cache_guard.insert(path, parent_id.clone());
+
+        Ok(parent_id)
+    }
+
+    pub async fn gdrive_get(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let url: String = format!(
+            "https://www.googleapis.com/drive/v3/files/{}?alt=media",
+            self.get_file_id_by_path(path).await?
+        );
 
-        let req = req
+        let req = self
+            .sign(Request::get(&url))
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
 
-    pub async fn onedrive_put(
+    pub async fn gdrive_update(
         &self,
         path: &str,
         size: Option<usize>,
         content_type: Option<&str>,
         body: AsyncBody,
     ) -> Result<Response<IncomingAsyncBody>> {
         let url = format!(
-            "https://graph.microsoft.com/v1.0/me/drive/root:{}:/content",
-            percent_encode_path(path)
+            "https://www.googleapis.com/upload/drive/v3/files/{}",
+            self.get_file_id_by_path(path).await?
         );
 
-        let mut req = Request::put(&url);
-
-        let auth_header_content = format!("Bearer {}", self.access_token);
-        req = req.header(header::AUTHORIZATION, auth_header_content);
+        let mut req = Request::patch(&url);
 
         if let Some(size) = size {
             req = req.header(header::CONTENT_LENGTH, size)
         }
 
         if let Some(mime) = content_type {
             req = req.header(header::CONTENT_TYPE, mime)
         }
 
-        let req = req.body(body).map_err(new_request_build_error)?;
+        let req = self.sign(req).body(body).map_err(new_request_build_error)?;
+
+        self.client.send(req).await
+    }
+
+    pub async fn gdrive_delete(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
+        let url = format!(
+            "https://www.googleapis.com/drive/v3/files/{}",
+            self.get_file_id_by_path(path).await?
+        );
+
+        let req = self
+            .sign(Request::delete(&url))
+            .body(AsyncBody::Empty)
+            .map_err(new_request_build_error)?;
 
         self.client.send(req).await
     }
+
+    fn sign(&self, mut req: Builder) -> Builder {
+        let auth_header_content = format!("Bearer {}", self.access_token);
+        req = req.header(header::AUTHORIZATION, auth_header_content);
+        req
+    }
+}
+
+// refer to https://developers.google.com/drive/api/reference/rest/v3/files#File
+#[derive(Deserialize)]
+struct GdriveFile {
+    id: String,
+}
+
+// refer to https://developers.google.com/drive/api/reference/rest/v3/files/list
+#[derive(Deserialize)]
+struct GdriveFileList {
+    files: Vec<GdriveFile>,
 }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/builder.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/builder.rs`

 * *Files 3% similar despite different names*

```diff
@@ -31,25 +31,24 @@
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
 /// - [x] read
 /// - [x] write
+/// - [x] list
 /// - [ ] copy
 /// - [ ] rename
-/// - [ ] list
 /// - [ ] ~~scan~~
 /// - [ ] ~~presign~~
 /// - [ ] blocking
 ///
 /// # Notes
 ///
 /// Currently, only OneDrive Personal is supported.
-/// For uploading, only files under 4MB are supported via the Simple Upload API (<https://learn.microsoft.com/en-us/onedrive/developer/rest-api/api/driveitem_put_content?view=odsp-graph-online>).
 ///
 /// # Configuration
 ///
 /// - `access_token`: set the access_token for Graph API
 /// - `root`: Set the work directory for backend
 ///
 /// You can refer to [`OnedriveBuilder`]'s docs for more information
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/onedrive/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/mod.rs`

 * *Files 5% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-mod builder;
-mod error;
+pub use backend::WebhdfsBuilder as Webhdfs;
 
-pub use builder::OnedriveBuilder as Onedrive;
+mod error;
+mod message;
+mod pager;
 mod writer;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/onedrive/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/writer.rs`

 * *Files 14% similar despite different names*

```diff
@@ -11,56 +11,56 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::OnedriveBackend;
+use super::core::*;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct OneDriveWriter {
-    backend: OnedriveBackend,
+pub struct WasabiWriter {
+    core: Arc<WasabiCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl OneDriveWriter {
-    pub fn new(backend: OnedriveBackend, op: OpWrite, path: String) -> Self {
-        OneDriveWriter { backend, op, path }
+impl WasabiWriter {
+    pub fn new(core: Arc<WasabiCore>, op: OpWrite, path: String) -> Self {
+        WasabiWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for OneDriveWriter {
+impl oio::Write for WasabiWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
         let resp = self
-            .backend
-            .onedrive_put(
+            .core
+            .put_object(
                 &self.path,
                 Some(bs.len()),
                 self.op.content_type(),
+                self.op.content_disposition(),
+                self.op.cache_control(),
                 AsyncBody::Bytes(bs),
             )
             .await?;
 
-        let status = resp.status();
-
-        match status {
-            // Typical response code: 201 Created
-            // Reference: https://learn.microsoft.com/en-us/onedrive/developer/rest-api/api/driveitem_put_content?view=odsp-graph-online#response
-            StatusCode::CREATED => {
+        match resp.status() {
+            StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/oss/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/oss/backend.rs`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 use http::StatusCode;
 use http::Uri;
 use log::debug;
 use reqsign::AliyunConfig;
 use reqsign::AliyunLoader;
 use reqsign::AliyunOssSigner;
 
+use super::appender::OssAppender;
 use super::core::*;
 use super::error::parse_error;
 use super::pager::OssPager;
 use super::writer::OssWriter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
@@ -437,14 +438,15 @@
 
 #[async_trait]
 impl Accessor for OssBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = OssWriter;
     type BlockingWriter = ();
+    type Appender = OssAppender;
     type Pager = OssPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Oss)
             .set_root(&self.core.root)
@@ -464,14 +466,19 @@
                 write_with_cache_control: true,
                 write_with_content_type: true,
                 write_without_content_length: true,
                 delete: true,
                 create_dir: true,
                 copy: true,
 
+                append: true,
+                append_with_cache_control: true,
+                append_with_content_type: true,
+                append_with_content_disposition: true,
+
                 list: true,
                 list_with_delimiter_slash: true,
                 list_without_delimiter: true,
 
                 presign: true,
                 presign_stat: true,
                 presign_read: true,
@@ -528,14 +535,21 @@
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         Ok((
             RpWrite::default(),
             OssWriter::new(self.core.clone(), path, args),
         ))
     }
 
+    async fn append(&self, path: &str, args: OpAppend) -> Result<(RpAppend, Self::Appender)> {
+        Ok((
+            RpAppend::default(),
+            OssAppender::new(self.core.clone(), path, args),
+        ))
+    }
+
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
         let resp = self.core.oss_copy_object(from, to).await?;
         let status = resp.status();
 
         match status {
             StatusCode::OK => {
                 resp.into_body().consume().await?;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/oss/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/oss/core.rs`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 use http::Response;
 use reqsign::AliyunCredential;
 use reqsign::AliyunLoader;
 use reqsign::AliyunOssSigner;
 use serde::Deserialize;
 use serde::Serialize;
 
+use crate::ops::OpAppend;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
 mod constants {
     pub const X_OSS_SERVER_SIDE_ENCRYPTION: &str = "x-oss-server-side-encryption";
 
@@ -179,14 +180,62 @@
             req = req.header(CACHE_CONTROL, cache_control)
         }
 
         // set sse headers
         req = self.insert_sse_headers(req);
 
         let req = req.body(body).map_err(new_request_build_error)?;
+        Ok(req)
+    }
+
+    /// Oss append object request
+    ///
+    /// # Note
+    ///
+    /// This request is used to append data to an existing object or create an appendable object.
+    /// So we must set the `append` and `position` header.
+    ///
+    /// https://www.alibabacloud.com/help/object-storage-service/latest/appendobject
+    pub fn oss_append_object_request(
+        &self,
+        path: &str,
+        position: u64,
+        size: usize,
+        args: &OpAppend,
+        body: AsyncBody,
+    ) -> Result<Request<AsyncBody>> {
+        let p = build_abs_path(&self.root, path);
+        let endpoint = self.get_endpoint(false);
+        let url = format!(
+            "{}/{}?append&position={}",
+            endpoint,
+            percent_encode_path(&p),
+            position
+        );
+
+        let mut req = Request::post(&url);
+
+        req = req.header(CONTENT_LENGTH, size);
+
+        if let Some(mime) = args.content_type() {
+            req = req.header(CONTENT_TYPE, mime);
+        }
+
+        if let Some(pos) = args.content_disposition() {
+            req = req.header(CONTENT_DISPOSITION, pos);
+        }
+
+        if let Some(cache_control) = args.cache_control() {
+            req = req.header(CACHE_CONTROL, cache_control)
+        }
+
+        // set sse headers
+        req = self.insert_sse_headers(req);
+
+        let req = req.body(body).map_err(new_request_build_error)?;
         Ok(req)
     }
 
     pub fn oss_get_object_request(
         &self,
         path: &str,
         range: BytesRange,
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/oss/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/oss/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/oss/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/sled/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -12,13 +12,9 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::OssBuilder as Oss;
 
-mod core;
-mod error;
-mod pager;
-mod writer;
+pub use backend::SledBuilder as Sled;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/oss/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/oss/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/oss/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/oss/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/redis/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/redis/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,14 @@
 
 /// [Redis](https://redis.io/) services support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
-/// - [x] read
-/// - [x] write
-/// - [ ] ~~list~~
-/// - [ ] scan
-/// - [ ] ~~presign~~
-/// - [ ] blocking
-///
 /// - [x] stat
 /// - [x] read
 /// - [x] write
 /// - [x] create_dir
 /// - [x] delete
 /// - [ ] copy
 /// - [ ] rename
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/redis/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::RedisBuilder as Redis;
+pub use backend::WebdavBuilder as Webdav;
+
+mod error;
+mod list_response;
+mod pager;
+mod writer;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/rocksdb/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/backend.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/rocksdb/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/rocksdb/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/s3/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/s3/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -367,18 +367,20 @@
             // Trim trailing `/` so that we can accept `http://127.0.0.1:9000/`
             self.endpoint = Some(endpoint.trim_end_matches('/').to_string())
         }
 
         self
     }
 
-    /// Region represent the signing region of this endpoint.
+    /// Region represent the signing region of this endpoint. This is required
+    /// if you are using the default AWS S3 endpoint.
     ///
+    /// If using a custom endpoint,
     /// - If region is set, we will take user's input first.
-    /// - If not, we will use `us-east-1` as default.
+    /// - If not, the default `us-east-1` will be used.
     pub fn region(&mut self, region: &str) -> &mut Self {
         if !region.is_empty() {
             self.region = Some(region.to_string())
         }
 
         self
     }
@@ -947,14 +949,15 @@
 
 #[async_trait]
 impl Accessor for S3Backend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = S3Writer;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = S3Pager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::S3)
             .set_root(&self.core.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/s3/compatible_services.md` & `opendal-0.35.0/local_dependencies/opendal/src/services/s3/compatible_services.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/s3/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/s3/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/s3/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/s3/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/s3/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/s3/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/s3/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/s3/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/s3/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/s3/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sftp/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/cos/backend.rs`

 * *Files 16% similar despite different names*

```diff
@@ -11,515 +11,477 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::cmp::min;
 use std::collections::HashMap;
 use std::fmt::Debug;
-use std::fmt::Formatter;
+use std::sync::Arc;
 
 use async_trait::async_trait;
-use bb8::PooledConnection;
-use futures::executor::block_on;
+use http::StatusCode;
+use http::Uri;
 use log::debug;
-use openssh::RemoteChild;
-use openssh::Session;
-use openssh::SessionBuilder;
-use openssh::Stdio;
-use openssh_sftp_client::Sftp;
-use owning_ref::OwningHandle;
-use tokio::sync::OnceCell;
-
-use super::error::is_not_found;
-use super::error::is_sftp_protocol_error;
-use super::error::SftpError;
-use super::pager::SftpPager;
-use super::utils::SftpReader;
-use super::writer::SftpWriter;
+use reqsign::TencentCosConfig;
+use reqsign::TencentCosCredentialLoader;
+use reqsign::TencentCosSigner;
+
+use super::core::CosCore;
+use super::error::parse_error;
+use super::pager::CosPager;
+use super::writer::CosWriter;
 use crate::ops::*;
 use crate::raw::*;
 use crate::*;
 
-/// SFTP services support. (only works on unix)
+/// Huawei Cloud COS services support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
-/// - [x] read
-/// - [x] write
-/// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] ~~presign~~
-/// - [ ] blocking
-///
 /// - [x] stat
 /// - [x] read
 /// - [x] write
 /// - [x] create_dir
 /// - [x] delete
-/// - [ ] copy
+/// - [x] copy
 /// - [ ] rename
 /// - [x] list
-/// - [ ] ~~scan~~
-/// - [ ] ~~presign~~
+/// - [x] scan
+/// - [ ] presign
 /// - [ ] blocking
 ///
 /// # Configuration
 ///
-/// - `endpoint`: Set the endpoint for connection
-/// - `root`: Set the work directory for backend, default to `/home/$USER/`
-/// - `user`: Set the login user
-/// - `key`: Set the public key for login
-///
-/// It doesn't support password login, you can use public key instead.
+/// - `root`: Set the work directory for backend
+/// - `bucket`: Set the container name for backend
+/// - `endpoint`: Customizable endpoint setting
+/// - `access_key_id`: Set the access_key_id for backend.
+/// - `secret_access_key`: Set the secret_access_key for backend.
 ///
-/// You can refer to [`SftpBuilder`]'s docs for more information
+/// You can refer to [`CosBuilder`]'s docs for more information
 ///
 /// # Example
 ///
 /// ## Via Builder
 ///
 /// ```no_run
 /// use anyhow::Result;
-/// use opendal::services::Ftp;
-/// use opendal::Object;
+/// use opendal::services::Cos;
 /// use opendal::Operator;
 ///
 /// #[tokio::main]
 /// async fn main() -> Result<()> {
 ///     // create backend builder
-///     let mut builder = Sftp::default();
+///     let mut builder = Cos::default();
 ///
-///     builder.endpoint("127.0.0.1").user("test").password("test");
+///     // set the storage bucket for OpenDAL
+///     builder.bucket("test");
+///     // set the endpoint for OpenDAL
+///     builder.endpoint("https://cos.ap-singapore.myqcloud.com");
+///     // Set the access_key_id and secret_access_key.
+///     //
+///     // OpenDAL will try load credential from the env.
+///     // If credential not set and no valid credential in env, OpenDAL will
+///     // send request without signing like anonymous user.
+///     builder.secret_id("secret_id");
+///     builder.secret_key("secret_access_key");
 ///
 ///     let op: Operator = Operator::new(builder)?.finish();
-///     let _obj: Object = op.object("test_file");
+///
 ///     Ok(())
 /// }
 /// ```
-
-#[derive(Default)]
-pub struct SftpBuilder {
-    endpoint: Option<String>,
+#[derive(Default, Clone)]
+pub struct CosBuilder {
     root: Option<String>,
-    user: Option<String>,
-    key: Option<String>,
+    endpoint: Option<String>,
+    secret_id: Option<String>,
+    secret_key: Option<String>,
+    bucket: Option<String>,
+    http_client: Option<HttpClient>,
+
+    disable_config_load: bool,
 }
 
-impl Debug for SftpBuilder {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+impl Debug for CosBuilder {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         f.debug_struct("Builder")
-            .field("endpoint", &self.endpoint)
             .field("root", &self.root)
+            .field("endpoint", &self.endpoint)
+            .field("secret_id", &"<redacted>")
+            .field("secret_key", &"<redacted>")
+            .field("bucket", &self.bucket)
             .finish()
     }
 }
 
-impl SftpBuilder {
-    /// set endpoint for sftp backend.
-    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
-        self.endpoint = if endpoint.is_empty() {
-            None
-        } else {
-            Some(endpoint.to_string())
-        };
+impl CosBuilder {
+    /// Set root of this backend.
+    ///
+    /// All operations will happen under this root.
+    pub fn root(&mut self, root: &str) -> &mut Self {
+        if !root.is_empty() {
+            self.root = Some(root.to_string())
+        }
 
         self
     }
 
-    /// set root path for sftp backend.
-    pub fn root(&mut self, root: &str) -> &mut Self {
-        self.root = if root.is_empty() {
-            None
-        } else {
-            Some(root.to_string())
-        };
+    /// Set endpoint of this backend.
+    ///
+    /// NOTE: no bucket or account id in endpoint, we will trim them if exists.
+    ///
+    /// # Examples
+    ///
+    /// - `https://cos.ap-singapore.myqcloud.com`
+    pub fn endpoint(&mut self, endpoint: &str) -> &mut Self {
+        if !endpoint.is_empty() {
+            self.endpoint = Some(endpoint.trim_end_matches('/').to_string());
+        }
 
         self
     }
 
-    /// set user for sftp backend.
-    pub fn user(&mut self, user: &str) -> &mut Self {
-        self.user = if user.is_empty() {
-            None
-        } else {
-            Some(user.to_string())
-        };
+    /// Set secret_id of this backend.
+    /// - If it is set, we will take user's input first.
+    /// - If not, we will try to load it from environment.
+    pub fn secret_id(&mut self, secret_id: &str) -> &mut Self {
+        if !secret_id.is_empty() {
+            self.secret_id = Some(secret_id.to_string());
+        }
 
         self
     }
 
-    /// set key path for sftp backend.
-    pub fn key(&mut self, key: &str) -> &mut Self {
-        self.key = if key.is_empty() {
-            None
-        } else {
-            Some(key.to_string())
-        };
+    /// Set secret_key of this backend.
+    /// - If it is set, we will take user's input first.
+    /// - If not, we will try to load it from environment.
+    pub fn secret_key(&mut self, secret_key: &str) -> &mut Self {
+        if !secret_key.is_empty() {
+            self.secret_key = Some(secret_key.to_string());
+        }
 
         self
     }
-}
 
-impl Builder for SftpBuilder {
-    const SCHEME: Scheme = Scheme::Sftp;
-    type Accessor = SftpBackend;
+    /// Set bucket of this backend.
+    /// The param is required.
+    pub fn bucket(&mut self, bucket: &str) -> &mut Self {
+        if !bucket.is_empty() {
+            self.bucket = Some(bucket.to_string());
+        }
 
-    fn build(&mut self) -> Result<Self::Accessor> {
-        debug!("sftp backend build started: {:?}", &self);
-        let endpoint = match self.endpoint.clone() {
-            Some(v) => v,
-            None => return Err(Error::new(ErrorKind::ConfigInvalid, "endpoint is empty")),
-        };
+        self
+    }
 
-        let user = match self.user.clone() {
-            Some(v) => v,
-            None => return Err(Error::new(ErrorKind::ConfigInvalid, "user is empty")),
-        };
+    /// Disable config load so that opendal will not load config from
+    /// environment.
+    ///
+    /// For examples:
+    ///
+    /// - envs like `TENCENTCLOUD_SECRET_ID`
+    pub fn disable_config_load(&mut self) -> &mut Self {
+        self.disable_config_load = true;
+        self
+    }
 
-        let root = self
-            .root
-            .clone()
-            .map(|r| normalize_root(r.as_str()))
-            .unwrap_or(format!("/home/{}/", user));
-
-        debug!("sftp backend finished: {:?}", &self);
-
-        Ok(SftpBackend {
-            endpoint,
-            root,
-            user,
-            key: self.key.clone(),
-            sftp: OnceCell::new(),
-        })
+    /// Specify the http client that used by this service.
+    ///
+    /// # Notes
+    ///
+    /// This API is part of OpenDAL's Raw API. `HttpClient` could be changed
+    /// during minor updates.
+    pub fn http_client(&mut self, client: HttpClient) -> &mut Self {
+        self.http_client = Some(client);
+        self
     }
+}
+
+impl Builder for CosBuilder {
+    const SCHEME: Scheme = Scheme::Cos;
+    type Accessor = CosBackend;
 
     fn from_map(map: HashMap<String, String>) -> Self {
-        let mut builder = SftpBuilder::default();
+        let mut builder = CosBuilder::default();
 
         map.get("root").map(|v| builder.root(v));
+        map.get("bucket").map(|v| builder.bucket(v));
         map.get("endpoint").map(|v| builder.endpoint(v));
-        map.get("user").map(|v| builder.user(v));
-        map.get("key").map(|v| builder.key(v));
+        map.get("secret_id").map(|v| builder.secret_id(v));
+        map.get("secret_key").map(|v| builder.secret_key(v));
 
         builder
     }
-}
 
-#[derive(Clone)]
-pub struct Manager {
-    endpoint: String,
-    user: String,
-    key: Option<String>,
-}
+    fn build(&mut self) -> Result<Self::Accessor> {
+        debug!("backend build started: {:?}", &self);
 
-pub struct Connection {
-    // the remote child owns the ref to session, so we need to use owning handle
-    // The session will only create one child, so we can make sure the child can live
-    // as long as the session. (the session will be dropped when the connection is dropped)
-    // Related: https://stackoverflow.com/a/47260399
-    child: OwningHandle<Box<Session>, Box<RemoteChild<'static>>>,
-    pub sftp: Sftp,
-}
+        let root = normalize_root(&self.root.take().unwrap_or_default());
+        debug!("backend use root {}", root);
 
-#[async_trait]
-impl bb8::ManageConnection for Manager {
-    type Connection = Connection;
-    type Error = SftpError;
-
-    async fn connect(&self) -> std::result::Result<Self::Connection, Self::Error> {
-        let mut session = SessionBuilder::default();
-
-        session.user(self.user.clone());
-
-        if let Some(key) = &self.key {
-            session.keyfile(key);
-        }
-
-        let session = session.connect(self.endpoint.clone()).await?;
-
-        let sess = Box::new(session);
-        let mut oref = OwningHandle::new_with_fn(sess, unsafe {
-            |x| {
-                Box::new(
-                    block_on(
-                        (*x).subsystem("sftp")
-                            .stdin(Stdio::piped())
-                            .stdout(Stdio::piped())
-                            .spawn(),
-                    )
-                    .unwrap(),
-                )
-            }
-        });
+        let bucket = match &self.bucket {
+            Some(bucket) => Ok(bucket.to_string()),
+            None => Err(
+                Error::new(ErrorKind::ConfigInvalid, "The bucket is misconfigured")
+                    .with_context("service", Scheme::Cos),
+            ),
+        }?;
+        debug!("backend use bucket {}", &bucket);
 
-        let sftp = Sftp::new(
-            oref.stdin().take().unwrap(),
-            oref.stdout().take().unwrap(),
-            Default::default(),
-        )
-        .await?;
+        let uri = match &self.endpoint {
+            Some(endpoint) => endpoint.parse::<Uri>().map_err(|err| {
+                Error::new(ErrorKind::ConfigInvalid, "endpoint is invalid")
+                    .with_context("service", Scheme::Cos)
+                    .with_context("endpoint", endpoint)
+                    .set_source(err)
+            }),
+            None => Err(Error::new(ErrorKind::ConfigInvalid, "endpoint is empty")
+                .with_context("service", Scheme::Cos)),
+        }?;
+
+        let scheme = match uri.scheme_str() {
+            Some(scheme) => scheme.to_string(),
+            None => "https".to_string(),
+        };
 
-        Ok(Connection { child: oref, sftp })
-    }
+        // If endpoint contains bucket name, we should trim them.
+        let endpoint = uri.host().unwrap().replace(&format!("//{bucket}."), "//");
+        debug!("backend use endpoint {}", &endpoint);
 
-    async fn is_valid(&self, conn: &mut Self::Connection) -> std::result::Result<(), Self::Error> {
-        conn.child.session().check().await?;
-        Ok(())
-    }
+        let client = if let Some(client) = self.http_client.take() {
+            client
+        } else {
+            HttpClient::new().map_err(|err| {
+                err.with_operation("Builder::build")
+                    .with_context("service", Scheme::Cos)
+            })?
+        };
 
-    /// Always allow reuse conn.
-    fn has_broken(&self, _: &mut Self::Connection) -> bool {
-        false
-    }
-}
+        let mut cfg = TencentCosConfig::default();
+        if !self.disable_config_load {
+            cfg = cfg.from_env();
+        }
 
-/// Backend is used to serve `Accessor` support for sftp.
-pub struct SftpBackend {
-    endpoint: String,
-    root: String,
-    user: String,
-    key: Option<String>,
-    sftp: OnceCell<bb8::Pool<Manager>>,
-}
+        if let Some(v) = self.secret_id.take() {
+            cfg.secret_id = Some(v);
+        }
+        if let Some(v) = self.secret_key.take() {
+            cfg.secret_key = Some(v);
+        }
+
+        let cred_loader = TencentCosCredentialLoader::new(client.client(), cfg);
 
-impl Debug for SftpBackend {
-    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("Backend").finish()
+        let signer = TencentCosSigner::new();
+
+        debug!("backend build finished");
+        Ok(CosBackend {
+            core: Arc::new(CosCore {
+                bucket: bucket.clone(),
+                root,
+                endpoint: format!("{}://{}.{}", &scheme, &bucket, &endpoint),
+                signer,
+                loader: cred_loader,
+                client,
+            }),
+        })
     }
 }
 
+/// Backend for Huaweicloud COS services.
+#[derive(Debug, Clone)]
+pub struct CosBackend {
+    core: Arc<CosCore>,
+}
+
 #[async_trait]
-impl Accessor for SftpBackend {
-    type Reader = SftpReader;
+impl Accessor for CosBackend {
+    type Reader = IncomingAsyncBody;
     type BlockingReader = ();
-    type Writer = SftpWriter;
+    type Writer = CosWriter;
     type BlockingWriter = ();
-    type Pager = SftpPager;
+    type Appender = ();
+    type Pager = CosPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
-        am.set_root(self.root.as_str())
-            .set_scheme(Scheme::Sftp)
+        am.set_scheme(Scheme::Cos)
+            .set_root(&self.core.root)
+            .set_name(&self.core.bucket)
             .set_capability(Capability {
                 stat: true,
+                stat_with_if_match: true,
+                stat_with_if_none_match: true,
 
                 read: true,
+                read_can_next: true,
+                read_with_range: true,
+                read_with_if_match: true,
+                read_with_if_none_match: true,
 
                 write: true,
-                create_dir: true,
+                write_with_content_type: true,
+                write_with_cache_control: true,
+
                 delete: true,
+                create_dir: true,
+                copy: true,
 
                 list: true,
-                list_with_limit: true,
                 list_with_delimiter_slash: true,
+                list_without_delimiter: true,
+
+                presign: true,
+                presign_stat: true,
+                presign_read: true,
+                presign_write: true,
 
                 ..Default::default()
             });
 
         am
     }
 
     async fn create_dir(&self, path: &str, _: OpCreateDir) -> Result<RpCreateDir> {
-        let client = self.sftp_connect().await?;
-        let mut fs = client.sftp.fs();
-        fs.set_cwd(self.root.clone());
-
-        let paths: Vec<&str> = path.split_inclusive('/').collect();
-        let mut current = self.root.clone();
-        for p in paths {
-            if p.is_empty() {
-                continue;
-            }
+        let mut req =
+            self.core
+                .cos_put_object_request(path, Some(0), None, None, AsyncBody::Empty)?;
+
+        self.core.sign(&mut req).await?;
+
+        let resp = self.core.send(req).await?;
 
-            current.push_str(p);
-            let res = fs.create_dir(p).await;
+        let status = resp.status();
 
-            if let Err(e) = res {
-                // ignore error if dir already exists
-                if !is_sftp_protocol_error(&e) {
-                    return Err(e.into());
-                }
+        match status {
+            StatusCode::CREATED | StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(RpCreateDir::default())
             }
-            fs.set_cwd(current.clone());
+            _ => Err(parse_error(resp).await?),
         }
-
-        return Ok(RpCreateDir::default());
     }
 
     async fn read(&self, path: &str, args: OpRead) -> Result<(RpRead, Self::Reader)> {
-        let client = self.sftp_connect().await?;
-
-        let mut fs = client.sftp.fs();
-        fs.set_cwd(self.root.clone());
-        let path = fs.canonicalize(path).await?;
-
-        let mut file = client.sftp.open(path.as_path()).await?;
-
-        let total_length = file.metadata().await?.len().ok_or(Error::new(
-            ErrorKind::NotFound,
-            format!("file not found: {}", path.to_str().unwrap()).as_str(),
-        ))?;
-
-        let br = args.range();
-        let (start, end) = match (br.offset(), br.size()) {
-            // Read a specific range.
-            (Some(offset), Some(size)) => (offset, min(offset + size, total_length)),
-            // Read from offset.
-            (Some(offset), None) => (offset, total_length),
-            // Read the last size bytes.
-            (None, Some(size)) => (
-                if total_length > size {
-                    total_length - size
-                } else {
-                    0
-                },
-                total_length,
-            ),
-            // Read the whole file.
-            (None, None) => (0, total_length),
-        };
+        let resp = self
+            .core
+            .cos_get_object(path, args.range(), args.if_match(), args.if_none_match())
+            .await?;
 
-        let r = SftpReader::new(self.sftp_connect_owned().await?, path, start, end).await?;
+        let status = resp.status();
 
-        Ok((RpRead::new(end - start), r))
+        match status {
+            StatusCode::OK | StatusCode::PARTIAL_CONTENT => {
+                let meta = parse_into_metadata(path, resp.headers())?;
+                Ok((RpRead::with_metadata(meta), resp.into_body()))
+            }
+            _ => Err(parse_error(resp).await?),
+        }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
         if args.content_length().is_none() {
             return Err(Error::new(
                 ErrorKind::Unsupported,
                 "write without content length is not supported",
             ));
         }
 
-        if let Some((dir, _)) = path.rsplit_once('/') {
-            self.create_dir(dir, OpCreateDir::default()).await?;
-        }
-
-        let path = format!("{}{}", self.root, path);
-
         Ok((
-            RpWrite::new(),
-            SftpWriter::new(self.sftp_connect_owned().await?, path),
+            RpWrite::default(),
+            CosWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
-    async fn stat(&self, path: &str, _: OpStat) -> Result<RpStat> {
-        let client = self.sftp_connect().await?;
-        let mut fs = client.sftp.fs();
-        fs.set_cwd(self.root.clone());
+    async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
+        let resp = self.core.cos_copy_object(from, to).await?;
 
-        let meta = fs.metadata(path).await?;
+        let status = resp.status();
 
-        Ok(RpStat::new(meta.into()))
+        match status {
+            StatusCode::OK => {
+                resp.into_body().consume().await?;
+                Ok(RpCopy::default())
+            }
+            _ => Err(parse_error(resp).await?),
+        }
     }
 
-    async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
-        let client = self.sftp_connect().await?;
-
-        let mut fs = client.sftp.fs();
-        fs.set_cwd(self.root.clone());
+    async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
+        // Stat root always returns a DIR.
+        if path == "/" {
+            return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
+        }
 
-        if path.ends_with('/') {
-            let file_path = format!("./{}", path);
-            let dir = match fs.open_dir(file_path.clone()).await {
-                Ok(dir) => dir,
-                Err(e) => {
-                    if is_not_found(&e) {
-                        return Ok(RpDelete::default());
-                    } else {
-                        return Err(e.into());
-                    }
-                }
-            }
-            .read_dir()
+        let resp = self
+            .core
+            .cos_head_object(path, args.if_match(), args.if_none_match())
             .await?;
 
-            for file in &dir {
-                let file_name = file.filename().to_str().unwrap();
-                if file_name == "." || file_name == ".." {
-                    continue;
-                }
-                let file_path = format!("{}{}", path, file_name);
-                self.delete(file_path.as_str(), OpDelete::default()).await?;
+        let status = resp.status();
+
+        // The response is very similar to azblob.
+        match status {
+            StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
+            StatusCode::NOT_FOUND if path.ends_with('/') => {
+                Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
             }
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
+    async fn delete(&self, path: &str, _: OpDelete) -> Result<RpDelete> {
+        let resp = self.core.cos_delete_object(path).await?;
 
-            match fs.remove_dir(path).await {
-                Err(e) if !is_not_found(&e) => {
-                    return Err(e.into());
-                }
-                _ => {}
+        let status = resp.status();
+
+        match status {
+            StatusCode::NO_CONTENT | StatusCode::ACCEPTED | StatusCode::NOT_FOUND => {
+                Ok(RpDelete::default())
             }
-        } else {
-            match fs.remove_file(path).await {
-                Err(e) if !is_not_found(&e) => {
-                    return Err(e.into());
-                }
-                _ => {}
+            _ => Err(parse_error(resp).await?),
+        }
+    }
+
+    async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
+        let mut req = match args.operation() {
+            PresignOperation::Stat(v) => {
+                self.core
+                    .cos_head_object_request(path, v.if_match(), v.if_none_match())?
             }
+            PresignOperation::Read(v) => self.core.cos_get_object_request(
+                path,
+                v.range(),
+                v.if_match(),
+                v.if_none_match(),
+            )?,
+            PresignOperation::Write(v) => self.core.cos_put_object_request(
+                path,
+                None,
+                v.content_type(),
+                v.cache_control(),
+                AsyncBody::Empty,
+            )?,
         };
+        self.core.sign_query(&mut req, args.expire()).await?;
+
+        // We don't need this request anymore, consume it directly.
+        let (parts, _) = req.into_parts();
 
-        Ok(RpDelete::default())
+        Ok(RpPresign::new(PresignedRequest::new(
+            parts.method,
+            parts.uri,
+            parts.headers,
+        )))
     }
 
     async fn list(&self, path: &str, args: OpList) -> Result<(RpList, Self::Pager)> {
-        let client = self.sftp_connect().await?;
-        let mut fs = client.sftp.fs();
-        fs.set_cwd(self.root.clone());
-
-        let file_path = format!("./{}", path);
-
-        let mut dir = match fs.open_dir(file_path.clone()).await {
-            Ok(dir) => dir,
-            Err(e) => {
-                if is_not_found(&e) {
-                    return Ok((RpList::default(), SftpPager::empty()));
-                } else {
-                    return Err(e.into());
-                }
-            }
-        };
-        let dir = dir.read_dir().await?;
-
         Ok((
             RpList::default(),
-            SftpPager::new(dir.into_inner(), path.to_owned(), args.limit()),
+            CosPager::new(self.core.clone(), path, args.delimiter(), args.limit()),
         ))
     }
 }
-
-impl SftpBackend {
-    async fn pool(&self) -> Result<&bb8::Pool<Manager>> {
-        let pool = self
-            .sftp
-            .get_or_try_init(|| async {
-                let manager = Manager {
-                    endpoint: self.endpoint.clone(),
-                    user: self.user.clone(),
-                    key: self.key.clone(),
-                };
-
-                bb8::Pool::builder().max_size(10).build(manager).await
-            })
-            .await?;
-
-        Ok(pool)
-    }
-
-    pub async fn sftp_connect(&self) -> Result<PooledConnection<'_, Manager>> {
-        let conn = self.pool().await?.get().await?;
-
-        Ok(conn)
-    }
-
-    pub async fn sftp_connect_owned(&self) -> Result<PooledConnection<'static, Manager>> {
-        let conn = self.pool().await?.get_owned().await?;
-
-        Ok(conn)
-    }
-}
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sftp/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/error.rs`

 * *Files 15% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use bb8::RunError;
 use openssh::Error as SshError;
-use openssh_sftp_client::{error::SftpErrorKind, Error as SftpClientError};
+use openssh_sftp_client::error::SftpErrorKind;
+use openssh_sftp_client::Error as SftpClientError;
 
-use crate::{Error, ErrorKind};
+use crate::Error;
+use crate::ErrorKind;
 
 #[derive(Debug)]
 pub enum SftpError {
     SftpClientError(SftpClientError),
     SshError(SshError),
 }
 
@@ -67,25 +68,14 @@
         match e {
             SftpError::SftpClientError(e) => e.into(),
             SftpError::SshError(e) => e.into(),
         }
     }
 }
 
-impl From<RunError<SftpError>> for Error {
-    fn from(e: RunError<SftpError>) -> Self {
-        match e {
-            RunError::User(err) => err.into(),
-            RunError::TimedOut => {
-                Error::new(ErrorKind::Unexpected, "connection request: timeout").set_temporary()
-            }
-        }
-    }
-}
-
 pub(super) fn is_not_found(e: &SftpClientError) -> bool {
     matches!(e, SftpClientError::SftpError(SftpErrorKind::NoSuchFile, _))
 }
 
 pub(super) fn is_sftp_protocol_error(e: &SftpClientError) -> bool {
     matches!(e, SftpClientError::SftpError(_, _))
 }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sftp/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sftp/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/pager.rs`

 * *Files 12% similar despite different names*

```diff
@@ -11,85 +11,69 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::pin::Pin;
+
 use async_trait::async_trait;
+use futures::StreamExt;
 use openssh_sftp_client::fs::DirEntry;
+use openssh_sftp_client::fs::ReadDir;
 
 use crate::raw::oio;
 use crate::Result;
 
 pub struct SftpPager {
-    dir: Box<[DirEntry]>,
-    path: String,
-    limit: Option<usize>,
-    complete: bool,
+    dir: Pin<Box<ReadDir>>,
+    prefix: String,
+    limit: usize,
 }
 
 impl SftpPager {
-    pub fn new(dir: Box<[DirEntry]>, path: String, limit: Option<usize>) -> Self {
-        Self {
-            dir,
-            path,
-            limit,
-            complete: false,
-        }
-    }
+    pub fn new(dir: ReadDir, path: String, limit: Option<usize>) -> Self {
+        let prefix = if path == "/" { "".to_owned() } else { path };
+
+        let limit = limit.unwrap_or(usize::MAX);
 
-    pub fn empty() -> Self {
-        Self {
-            dir: Box::new([]),
-            path: String::new(),
-            limit: None,
-            complete: true,
+        SftpPager {
+            dir: Box::pin(dir),
+            prefix,
+            limit,
         }
     }
 }
 
 #[async_trait]
 impl oio::Page for SftpPager {
     async fn next(&mut self) -> Result<Option<Vec<oio::Entry>>> {
-        if self.complete {
+        if self.limit == 0 {
             return Ok(None);
         }
 
-        // when listing the root directory, the prefix should be empty
-        if self.path == "/" {
-            self.path = "".to_owned();
-        }
-
-        let iter = self
-            .dir
-            .iter()
-            .filter(|e| {
-                // filter out "." and ".."
-                e.filename().to_str().unwrap() != "." && e.filename().to_str().unwrap() != ".."
-            })
-            .map(|e| map_entry(self.path.clone(), e.clone()));
-
-        let v: Vec<oio::Entry> = if let Some(limit) = self.limit {
-            iter.take(limit).collect()
-        } else {
-            iter.collect()
-        };
-
-        self.complete = true;
+        let item = self.dir.next().await;
 
-        if v.is_empty() {
-            Ok(None)
-        } else {
-            Ok(Some(v))
+        match item {
+            Some(Ok(e)) => {
+                if e.filename().to_str() == Some(".") || e.filename().to_str() == Some("..") {
+                    self.next().await
+                } else {
+                    self.limit -= 1;
+                    Ok(Some(vec![map_entry(self.prefix.as_str(), e.clone())]))
+                }
+            }
+            Some(Err(e)) => Err(e.into()),
+            None => Ok(None),
         }
     }
 }
 
-fn map_entry(prefix: String, value: DirEntry) -> oio::Entry {
+fn map_entry(prefix: &str, value: DirEntry) -> oio::Entry {
     let path = format!(
         "{}{}{}",
         prefix,
         value.filename().to_str().unwrap(),
         if value.file_type().unwrap().is_dir() {
             "/"
         } else {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sftp/utils.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/utils.rs`

 * *Files 17% similar despite different names*

```diff
@@ -12,73 +12,88 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::io::SeekFrom;
-use std::path::PathBuf;
 use std::pin::Pin;
 use std::task::Context;
 use std::task::Poll;
 
 use async_compat::Compat;
-use bb8::PooledConnection;
-use futures::executor::block_on;
+use futures::AsyncBufRead;
+use futures::AsyncRead;
+use futures::AsyncSeek;
+use openssh_sftp_client::file::File;
 use openssh_sftp_client::file::TokioCompatFile;
 use openssh_sftp_client::metadata::MetaData as SftpMeta;
-use owning_ref::OwningHandle;
 
-use super::backend::Manager;
 use crate::raw::oio;
 use crate::raw::oio::into_reader::FdReader;
 use crate::raw::oio::ReadExt;
 use crate::EntryMode;
 use crate::Metadata;
 use crate::Result;
 
-pub struct SftpReader {
-    // similar situation to connection struct
-    // We can make sure the file can live as long as the connection.
-    file: OwningHandle<
-        Box<PooledConnection<'static, Manager>>,
-        Box<FdReader<Compat<TokioCompatFile<'static>>>>,
-    >,
+pub struct SftpReaderInner {
+    file: Pin<Box<Compat<TokioCompatFile>>>,
 }
+pub type SftpReader = FdReader<SftpReaderInner>;
 
-impl SftpReader {
-    pub async fn new(
-        conn: PooledConnection<'static, Manager>,
-        path: PathBuf,
-        start: u64,
-        end: u64,
-    ) -> Result<Self> {
-        let mut file = OwningHandle::new_with_fn(Box::new(conn), |conn| unsafe {
-            let file = block_on((*conn).sftp.open(path)).unwrap();
-            let f = Compat::new(TokioCompatFile::from(file));
-            Box::new(oio::into_reader::from_fd(f, start, end))
-        });
+impl SftpReaderInner {
+    pub async fn new(file: File) -> Self {
+        let file = Compat::new(file.into());
+        Self {
+            file: Box::pin(file),
+        }
+    }
+}
 
-        file.seek(SeekFrom::Start(0)).await?;
+impl SftpReader {
+    /// Create a new reader from a file, starting at the given offset and ending at the given offset.
+    pub async fn new(file: File, start: u64, end: u64) -> Result<Self> {
+        let file = SftpReaderInner::new(file).await;
+        let mut r = oio::into_reader::from_fd(file, start, end);
+        r.seek(SeekFrom::Start(0)).await?;
+        Ok(r)
+    }
+}
 
-        Ok(SftpReader { file })
+impl AsyncRead for SftpReaderInner {
+    fn poll_read(
+        self: Pin<&mut Self>,
+        cx: &mut Context,
+        buf: &mut [u8],
+    ) -> Poll<std::io::Result<usize>> {
+        let this = self.get_mut();
+        Pin::new(&mut this.file).poll_read(cx, buf)
     }
 }
 
-impl oio::Read for SftpReader {
-    fn poll_read(&mut self, cx: &mut Context, buf: &mut [u8]) -> Poll<Result<usize>> {
-        Pin::new(&mut *self.file).poll_read(cx, buf)
+impl AsyncBufRead for SftpReaderInner {
+    fn poll_fill_buf(self: Pin<&mut Self>, cx: &mut Context) -> Poll<std::io::Result<&[u8]>> {
+        let this = self.get_mut();
+        Pin::new(&mut this.file).poll_fill_buf(cx)
     }
 
-    fn poll_seek(&mut self, cx: &mut Context<'_>, pos: SeekFrom) -> Poll<Result<u64>> {
-        Pin::new(&mut *self.file).poll_seek(cx, pos)
+    fn consume(self: Pin<&mut Self>, amt: usize) {
+        let this = self.get_mut();
+        Pin::new(&mut this.file).consume(amt)
     }
+}
 
-    fn poll_next(&mut self, cx: &mut Context<'_>) -> Poll<Option<Result<bytes::Bytes>>> {
-        Pin::new(&mut *self.file).poll_next(cx)
+impl AsyncSeek for SftpReaderInner {
+    fn poll_seek(
+        self: Pin<&mut Self>,
+        cx: &mut Context,
+        pos: SeekFrom,
+    ) -> Poll<std::io::Result<u64>> {
+        let this = self.get_mut();
+        Pin::new(&mut this.file).poll_seek(cx, pos)
     }
 }
 
 impl From<SftpMeta> for Metadata {
     fn from(meta: SftpMeta) -> Self {
         let mode = meta
             .file_type()
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sftp/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/sftp/writer.rs`

 * *Files 12% similar despite different names*

```diff
@@ -12,38 +12,36 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
-use bb8::PooledConnection;
 use bytes::Bytes;
+use openssh_sftp_client::file::File;
 
-use super::backend::Manager;
 use crate::raw::oio;
-use crate::{Error, ErrorKind, Result};
+use crate::Error;
+use crate::ErrorKind;
+use crate::Result;
 
 pub struct SftpWriter {
-    conn: PooledConnection<'static, Manager>,
-    path: String,
+    file: File,
 }
 
 impl SftpWriter {
-    pub fn new(conn: PooledConnection<'static, Manager>, path: String) -> Self {
-        SftpWriter { conn, path }
+    pub fn new(file: File) -> Self {
+        SftpWriter { file }
     }
 }
 
 #[async_trait]
 impl oio::Write for SftpWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let mut file = self.conn.sftp.create(&self.path).await?;
-
-        file.write_all(&bs).await?;
+        self.file.write_all(&bs).await?;
 
         Ok(())
     }
 
     async fn abort(&mut self) -> Result<()> {
         Err(Error::new(
             ErrorKind::Unsupported,
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sled/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/sled/backend.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,14 @@
 
 /// Sled service support.
 ///
 /// # Capabilities
 ///
 /// This service can be used to:
 ///
-/// - [x] read
-/// - [x] write
-/// - [ ] ~~list~~
-/// - [ ] scan
-/// - [ ] ~~presign~~
-/// - [x] blocking
-///
 /// - [x] stat
 /// - [x] read
 /// - [x] write
 /// - [x] create_dir
 /// - [x] delete
 /// - [ ] copy
 /// - [ ] rename
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/sled/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/gdrive/mod.rs`

 * *Files 21% similar despite different names*

```diff
@@ -12,9 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
+mod builder;
+mod core;
+mod error;
 
-pub use backend::SledBuilder as Sled;
+pub use builder::GdriveBuilder as Gdrive;
+mod writer;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/supabase/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
 #[async_trait]
 impl Accessor for SupabaseBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = SupabaseWriter;
     type BlockingWriter = ();
+    type Appender = ();
     // todo: implement Pager to support list and scan
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Supabase)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/supabase/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/core.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/supabase/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/supabase/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/supabase/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/supabase/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/backend.rs`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,39 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use async_trait::async_trait;
-use http::{header, Request, Response, StatusCode};
 use std::fmt::Debug;
 
-use crate::{
-    ops::{OpRead, OpWrite},
-    raw::{
-        new_request_build_error, parse_into_metadata, Accessor, AccessorInfo, AsyncBody,
-        HttpClient, IncomingAsyncBody, RpRead, RpWrite,
-    },
-    types::Result,
-    Capability, Error, ErrorKind,
-};
-
-use super::{error::parse_error, writer::VercelArtifactsWriter};
+use async_trait::async_trait;
+use http::header;
+use http::Request;
+use http::Response;
+use http::StatusCode;
+
+use super::error::parse_error;
+use super::writer::VercelArtifactsWriter;
+use crate::ops::OpRead;
+use crate::ops::OpWrite;
+use crate::raw::new_request_build_error;
+use crate::raw::parse_into_metadata;
+use crate::raw::Accessor;
+use crate::raw::AccessorInfo;
+use crate::raw::AsyncBody;
+use crate::raw::HttpClient;
+use crate::raw::IncomingAsyncBody;
+use crate::raw::RpRead;
+use crate::raw::RpWrite;
+use crate::types::Result;
+use crate::Capability;
+use crate::Error;
+use crate::ErrorKind;
 
 #[derive(Clone)]
 pub struct VercelArtifactsBackend {
     pub(crate) access_token: String,
     pub(crate) client: HttpClient,
 }
 
@@ -47,14 +57,15 @@
 
 #[async_trait]
 impl Accessor for VercelArtifactsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = VercelArtifactsWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = ();
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(crate::Scheme::VercelArtifacts)
             .set_capability(Capability {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/builder.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/vercel_artifacts/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -892,14 +892,15 @@
 
 #[async_trait]
 impl Accessor for WasabiBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = WasabiWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = WasabiPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Wasabi)
             .set_root(&self.core.root)
@@ -970,14 +971,21 @@
                 Ok((RpRead::with_metadata(meta), resp.into_body()))
             }
             _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn write(&self, path: &str, args: OpWrite) -> Result<(RpWrite, Self::Writer)> {
+        if args.content_length().is_none() {
+            return Err(Error::new(
+                ErrorKind::Unsupported,
+                "write without content length is not supported",
+            ));
+        }
+
         Ok((
             RpWrite::default(),
             WasabiWriter::new(self.core.clone(), args, path.to_string()),
         ))
     }
 
     async fn copy(&self, from: &str, to: &str, _args: OpCopy) -> Result<RpCopy> {
@@ -999,15 +1007,15 @@
 
     async fn stat(&self, path: &str, args: OpStat) -> Result<RpStat> {
         // Stat root always returns a DIR.
         if path == "/" {
             return Ok(RpStat::new(Metadata::new(EntryMode::DIR)));
         }
 
-        let resp = self.core.head_object(path, args.if_none_match()).await?;
+        let resp = self.core.head_object(path, &args).await?;
 
         let status = resp.status();
 
         match status {
             StatusCode::OK => parse_into_metadata(path, resp.headers()).map(RpStat::new),
             StatusCode::NOT_FOUND if path.ends_with('/') => {
                 Ok(RpStat::new(Metadata::new(EntryMode::DIR)))
@@ -1033,15 +1041,15 @@
             WasabiPager::new(self.core.clone(), path, args.delimiter(), args.limit()),
         ))
     }
 
     async fn presign(&self, path: &str, args: OpPresign) -> Result<RpPresign> {
         // We will not send this request out, just for signing.
         let mut req = match args.operation() {
-            PresignOperation::Stat(v) => self.core.head_object_request(path, v.if_none_match())?,
+            PresignOperation::Stat(v) => self.core.head_object_request(path, v)?,
             PresignOperation::Read(v) => self.core.get_object_request(
                 path,
                 v.range(),
                 v.override_content_disposition(),
                 v.override_cache_control(),
                 v.if_none_match(),
             )?,
@@ -1148,15 +1156,15 @@
     #[test]
     fn test_build_endpoint() {
         let _ = tracing_subscriber::fmt().with_test_writer().try_init();
 
         let endpoint_cases = vec![
             Some("s3.wasabisys.com"),
             Some("https://s3.wasabisys.com"),
-            Some("https://s3.us-east-2.amazonaws.com"),
+            Some("https://s3.us-east-2.wasabisys.com"),
             None,
         ];
 
         for endpoint in &endpoint_cases {
             let mut b = WasabiBuilder::default();
             b.bucket("test");
             if let Some(endpoint) = endpoint {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/core.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/core.rs`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 use http::Response;
 use reqsign::AwsCredential;
 use reqsign::AwsLoader;
 use reqsign::AwsV4Signer;
 use serde::Deserialize;
 use serde::Serialize;
 
+use crate::ops::OpStat;
 use crate::raw::*;
 use crate::*;
 
 mod constants {
     pub const X_AMZ_COPY_SOURCE: &str = "x-amz-copy-source";
 
     pub const X_AMZ_SERVER_SIDE_ENCRYPTION: &str = "x-amz-server-side-encryption";
@@ -203,29 +204,29 @@
         }
 
         req
     }
 }
 
 impl WasabiCore {
-    pub fn head_object_request(
-        &self,
-        path: &str,
-        if_none_match: Option<&str>,
-    ) -> Result<Request<AsyncBody>> {
+    pub fn head_object_request(&self, path: &str, args: &OpStat) -> Result<Request<AsyncBody>> {
         let p = build_abs_path(&self.root, path);
 
         let url = format!("{}/{}", self.endpoint, percent_encode_path(&p));
 
         let mut req = Request::head(&url);
 
         req = self.insert_sse_headers(req, false);
 
-        if let Some(if_none_match) = if_none_match {
-            req = req.header(http::header::IF_NONE_MATCH, if_none_match);
+        if let Some(v) = args.if_match() {
+            req = req.header(http::header::IF_MATCH, v);
+        }
+
+        if let Some(v) = args.if_none_match() {
+            req = req.header(http::header::IF_NONE_MATCH, v);
         }
 
         let req = req
             .body(AsyncBody::Empty)
             .map_err(new_request_build_error)?;
 
         Ok(req)
@@ -342,17 +343,17 @@
 
         Ok(req)
     }
 
     pub async fn head_object(
         &self,
         path: &str,
-        if_none_match: Option<&str>,
+        args: &OpStat,
     ) -> Result<Response<IncomingAsyncBody>> {
-        let mut req = self.head_object_request(path, if_none_match)?;
+        let mut req = self.head_object_request(path, args)?;
 
         self.sign(&mut req).await?;
 
         self.send(req).await
     }
 
     pub async fn delete_object(&self, path: &str) -> Result<Response<IncomingAsyncBody>> {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/error.rs`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,17 @@
 pub async fn parse_error(resp: Response<IncomingAsyncBody>) -> Result<Error> {
     let (parts, body) = resp.into_parts();
     let bs = body.bytes().await?;
 
     let (mut kind, mut retryable) = match parts.status {
         StatusCode::NOT_FOUND => (ErrorKind::NotFound, false),
         StatusCode::FORBIDDEN => (ErrorKind::PermissionDenied, false),
-        StatusCode::PRECONDITION_FAILED => (ErrorKind::ConditionNotMatch, false),
+        StatusCode::PRECONDITION_FAILED | StatusCode::NOT_MODIFIED => {
+            (ErrorKind::ConditionNotMatch, false)
+        }
         StatusCode::INTERNAL_SERVER_ERROR
         | StatusCode::BAD_GATEWAY
         | StatusCode::SERVICE_UNAVAILABLE
         | StatusCode::GATEWAY_TIMEOUT => (ErrorKind::Unexpected, true),
         _ => (ErrorKind::Unexpected, false),
     };
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/wasabi/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/wasabi/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -11,75 +11,59 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
-use std::sync::Arc;
-
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::core::*;
+use super::backend::WebdavBackend;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WasabiWriter {
-    core: Arc<WasabiCore>,
+pub struct WebdavWriter {
+    backend: WebdavBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl WasabiWriter {
-    pub fn new(core: Arc<WasabiCore>, op: OpWrite, path: String) -> Self {
-        WasabiWriter { core, op, path }
+impl WebdavWriter {
+    pub fn new(backend: WebdavBackend, op: OpWrite, path: String) -> Self {
+        WebdavWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WasabiWriter {
+impl oio::Write for WebdavWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        if self.op.content_length().unwrap_or_default() == bs.len() as u64 {
-            let resp = self
-                .core
-                .put_object(
-                    &self.path,
-                    Some(bs.len()),
-                    self.op.content_type(),
-                    self.op.content_disposition(),
-                    self.op.cache_control(),
-                    AsyncBody::Bytes(bs),
-                )
-                .await?;
-
-            match resp.status() {
-                StatusCode::CREATED | StatusCode::OK => {
-                    resp.into_body().consume().await?;
-                    Ok(())
-                }
-                _ => Err(parse_error(resp).await?),
-            }
-        } else {
-            let resp = self
-                .core
-                .append_object(&self.path, Some(bs.len()), AsyncBody::Bytes(bs))
-                .await?;
-
-            match resp.status() {
-                StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
-                    resp.into_body().consume().await?;
-                    Ok(())
-                }
-                _ => Err(parse_error(resp).await?),
+        let resp = self
+            .backend
+            .webdav_put(
+                &self.path,
+                Some(bs.len()),
+                self.op.content_type(),
+                self.op.content_disposition(),
+                AsyncBody::Bytes(bs),
+            )
+            .await?;
+
+        let status = resp.status();
+
+        match status {
+            StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
+                resp.into_body().consume().await?;
+                Ok(())
             }
+            _ => Err(parse_error(resp).await?),
         }
     }
 
     async fn abort(&mut self) -> Result<()> {
         Ok(())
     }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webdav/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -258,14 +258,15 @@
 
 #[async_trait]
 impl Accessor for WebdavBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = WebdavWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = WebdavPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut ma = AccessorInfo::default();
         ma.set_scheme(Scheme::Webdav)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webdav/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx-with-basic-auth.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/fixtures/nginx.conf`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webdav/list_response.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/list_response.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webdav/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webdav/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webdav/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/writer.rs`

 * *Files 18% similar despite different names*

```diff
@@ -15,51 +15,51 @@
 // specific language governing permissions and limitations
 // under the License.
 
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::WebdavBackend;
+use super::backend::WebhdfsBackend;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WebdavWriter {
-    backend: WebdavBackend,
+pub struct WebhdfsWriter {
+    backend: WebhdfsBackend,
 
     op: OpWrite,
     path: String,
 }
 
-impl WebdavWriter {
-    pub fn new(backend: WebdavBackend, op: OpWrite, path: String) -> Self {
-        WebdavWriter { backend, op, path }
+impl WebhdfsWriter {
+    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
+        WebhdfsWriter { backend, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WebdavWriter {
+impl oio::Write for WebhdfsWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let resp = self
+        let req = self
             .backend
-            .webdav_put(
+            .webhdfs_create_object_request(
                 &self.path,
                 Some(bs.len()),
                 self.op.content_type(),
-                self.op.content_disposition(),
                 AsyncBody::Bytes(bs),
             )
             .await?;
 
-        let status = resp.status();
+        let resp = self.backend.client.send(req).await?;
 
+        let status = resp.status();
         match status {
-            StatusCode::CREATED | StatusCode::OK | StatusCode::NO_CONTENT => {
+            StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
     }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/backend.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/backend.rs`

 * *Files 1% similar despite different names*

```diff
@@ -459,14 +459,15 @@
 
 #[async_trait]
 impl Accessor for WebhdfsBackend {
     type Reader = IncomingAsyncBody;
     type BlockingReader = ();
     type Writer = WebhdfsWriter;
     type BlockingWriter = ();
+    type Appender = ();
     type Pager = WebhdfsPager;
     type BlockingPager = ();
 
     fn info(&self) -> AccessorInfo {
         let mut am = AccessorInfo::default();
         am.set_scheme(Scheme::Webhdfs)
             .set_root(&self.root)
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/message.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/message.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/cos/mod.rs`

 * *Files 13% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 mod backend;
-pub use backend::WebhdfsBuilder as Webhdfs;
+pub use backend::CosBuilder as Cos;
 
+mod core;
 mod error;
-mod message;
 mod pager;
 mod writer;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/pager.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/webhdfs/pager.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/services/webhdfs/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/services/cos/writer.rs`

 * *Files 11% similar despite different names*

```diff
@@ -11,53 +11,56 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::sync::Arc;
+
 use async_trait::async_trait;
 use bytes::Bytes;
 use http::StatusCode;
 
-use super::backend::WebhdfsBackend;
+use super::core::CosCore;
 use super::error::parse_error;
 use crate::ops::OpWrite;
 use crate::raw::*;
 use crate::*;
 
-pub struct WebhdfsWriter {
-    backend: WebhdfsBackend,
+pub struct CosWriter {
+    core: Arc<CosCore>,
 
     op: OpWrite,
     path: String,
 }
 
-impl WebhdfsWriter {
-    pub fn new(backend: WebhdfsBackend, op: OpWrite, path: String) -> Self {
-        WebhdfsWriter { backend, op, path }
+impl CosWriter {
+    pub fn new(core: Arc<CosCore>, op: OpWrite, path: String) -> Self {
+        CosWriter { core, op, path }
     }
 }
 
 #[async_trait]
-impl oio::Write for WebhdfsWriter {
+impl oio::Write for CosWriter {
     async fn write(&mut self, bs: Bytes) -> Result<()> {
-        let req = self
-            .backend
-            .webhdfs_create_object_request(
-                &self.path,
-                Some(bs.len()),
-                self.op.content_type(),
-                AsyncBody::Bytes(bs),
-            )
-            .await?;
+        let mut req = self.core.cos_put_object_request(
+            &self.path,
+            Some(bs.len()),
+            self.op.content_type(),
+            self.op.cache_control(),
+            AsyncBody::Bytes(bs),
+        )?;
+
+        self.core.sign(&mut req).await?;
 
-        let resp = self.backend.client.send(req).await?;
+        let resp = self.core.send(req).await?;
 
         let status = resp.status();
+
         match status {
             StatusCode::CREATED | StatusCode::OK => {
                 resp.into_body().consume().await?;
                 Ok(())
             }
             _ => Err(parse_error(resp).await?),
         }
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/builder.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/builder.rs`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
 use std::collections::HashMap;
-use std::env;
 
 use crate::raw::*;
 use crate::*;
 
 /// Builder is used to set up a real underlying service, i.e. storage accessor.
 ///
 /// One builder is usually used by [`Operator`] during its initialization.
@@ -41,39 +40,14 @@
     const SCHEME: Scheme;
     /// The accessor that built by this builder.
     type Accessor: Accessor;
 
     /// Construct a builder from given map which contains several parameters needed by underlying service.
     fn from_map(map: HashMap<String, String>) -> Self;
 
-    /// Construct a builder from given iterator.
-    fn from_iter(iter: impl Iterator<Item = (String, String)>) -> Self
-    where
-        Self: Sized,
-    {
-        Self::from_map(iter.collect())
-    }
-
-    /// Construct a builder from envs. Please note that the env should begin with `opendal_{schema_name}_`.
-    fn from_env() -> Self
-    where
-        Self: Sized,
-    {
-        let prefix = format!("opendal_{}_", Self::SCHEME);
-        let envs = env::vars()
-            .filter_map(move |(k, v)| {
-                k.to_lowercase()
-                    .strip_prefix(&prefix)
-                    .map(|k| (k.to_string(), v))
-            })
-            .collect();
-
-        Self::from_map(envs)
-    }
-
     /// Consume the accessor builder to build a service.
     fn build(&mut self) -> Result<Self::Accessor>;
 }
 
 /// Dummy implementation of builder
 impl Builder for () {
     const SCHEME: Scheme = Scheme::Custom("dummy");
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/capability.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/capability.rs`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,23 @@
     /// If operator supports write with content type natively, it will be true.
     pub write_with_content_type: bool,
     /// If operator supports write with content disposition natively, it will be true.
     pub write_with_content_disposition: bool,
     /// If operator supports write with cache control natively, it will be true.
     pub write_with_cache_control: bool,
 
+    /// If operator supports append natively, it will be true.
+    pub append: bool,
+    /// If operator supports append with content type natively, it will be true.
+    pub append_with_content_type: bool,
+    /// If operator supports append with content disposition natively, it will be true.
+    pub append_with_content_disposition: bool,
+    /// If operator supports append with cache control natively, it will be true.
+    pub append_with_cache_control: bool,
+
     /// If operator supports create dir natively, it will be true.
     pub create_dir: bool,
 
     /// If operator supports delete natively, it will be true.
     pub delete: bool,
 
     /// If operator supports copy natively, it will be true.
@@ -138,14 +147,17 @@
         }
         if self.read {
             s.push("Read");
         }
         if self.write {
             s.push("Write");
         }
+        if self.append {
+            s.push("Append");
+        }
         if self.create_dir {
             s.push("CreateDir");
         }
         if self.delete {
             s.push("Delete");
         }
         if self.copy {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/entry.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/entry.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/error.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/error.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/list.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/list.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/metadata.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/metadata.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/mod.rs`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 pub use reader::BlockingReader;
 pub use reader::Reader;
 
 mod writer;
 pub use writer::BlockingWriter;
 pub use writer::Writer;
 
+mod appender;
+pub use appender::Appender;
+
 mod list;
 pub use list::BlockingLister;
 pub use list::Lister;
 
 mod operator;
 pub use operator::BlockingOperator;
 pub use operator::Operator;
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/mode.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/mode.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/operator/blocking_operator.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/operator/metadata.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/operator/metadata.rs`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,19 @@
     }
 
     /// Check if current backend supports [`Accessor::write`] or not.
     pub fn can_write(&self) -> bool {
         self.0.capability().write
     }
 
+    /// Check if current backend supports [`Accessor::append`] or not.
+    pub fn can_append(&self) -> bool {
+        self.0.capability().append
+    }
+
     /// Check if current backend supports [`Accessor::copy`] or not.
     pub fn can_copy(&self) -> bool {
         self.0.capability().copy
     }
 
     /// Check if current backend supports [`Accessor::rename`] or not.
     pub fn can_rename(&self) -> bool {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/operator/mod.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/operator/operator.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/operator/operator.rs`

 * *Files 2% similar despite different names*

```diff
@@ -646,14 +646,40 @@
             path,
             OpWrite::new().with_content_length(bs.len() as u64),
             bs,
         )
         .await
     }
 
+    /// Append bytes into path.
+    ///
+    /// # Notes
+    ///
+    /// - Append will make sure all bytes has been written, or an error will be returned.
+    /// - Append will create the file if it does not exist.
+    /// - Append always write bytes to the end of the file.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    /// use bytes::Bytes;
+    ///
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// op.append("path/to/file", vec![0; 4096]).await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn append(&self, path: &str, bs: impl Into<Bytes>) -> Result<()> {
+        let bs = bs.into();
+        self.append_with(path, OpAppend::new(), bs).await
+    }
+
     /// Copy a file from `from` to `to`.
     ///
     /// # Notes
     ///
     /// - `from` and `to` must be a file.
     /// - `to` will be overwritten if it exists.
     /// - If `from` and `to` are the same,  an `IsSameFile` error will occur.
@@ -873,14 +899,124 @@
             .await?;
         w.write(bs).await?;
         w.close().await?;
 
         Ok(())
     }
 
+    /// Append multiple bytes into path.
+    ///
+    /// Refer to [`Appender`] for more details.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    /// use bytes::Bytes;
+    ///
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// let mut a = op.appender("path/to/file").await?;
+    /// a.append(vec![0; 4096]).await?;
+    /// a.append(vec![1; 4096]).await?;
+    /// a.close().await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn appender(&self, path: &str) -> Result<Appender> {
+        self.appender_with(path, OpAppend::default()).await
+    }
+
+    /// Append multiple bytes into path with extra options.
+    ///
+    /// Refer to [`Appender`] for more details.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    /// use bytes::Bytes;
+    /// use opendal::ops::OpAppend;
+    ///
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// let args = OpAppend::new().with_content_type("application/octet-stream");
+    /// let mut a = op.appender_with("path/to/file", args).await?;
+    /// a.append(vec![0; 4096]).await?;
+    /// a.append(vec![1; 4096]).await?;
+    /// a.close().await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn appender_with(&self, path: &str, args: OpAppend) -> Result<Appender> {
+        let path = normalize_path(path);
+
+        if !validate_path(&path, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "append path is a directory")
+                    .with_operation("Operator::appender")
+                    .with_context("service", self.inner().info().scheme().into_static())
+                    .with_context("path", &path),
+            );
+        }
+
+        Appender::create(self.inner().clone(), &path, args).await
+    }
+
+    /// Append bytes with extra options.
+    ///
+    /// # Notes
+    ///
+    /// - Append will make sure all bytes has been written, or an error will be returned.
+    /// - Append will create the file if it does not exist.
+    /// - Append always write bytes to the end of the file.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// # use std::io::Result;
+    /// # use opendal::Operator;
+    /// use bytes::Bytes;
+    /// use opendal::ops::OpAppend;
+    ///
+    /// # #[tokio::main]
+    /// # async fn test(op: Operator) -> Result<()> {
+    /// let bs = b"hello, world!".to_vec();
+    /// let args = OpAppend::new().with_content_type("text/plain");
+    /// let _ = op.append_with("path/to/file", args, bs).await?;
+    /// # Ok(())
+    /// # }
+    /// ```
+    pub async fn append_with(
+        &self,
+        path: &str,
+        args: OpAppend,
+        bs: impl Into<Bytes>,
+    ) -> Result<()> {
+        let path = normalize_path(path);
+
+        if !validate_path(&path, EntryMode::FILE) {
+            return Err(
+                Error::new(ErrorKind::IsADirectory, "append path is a directory")
+                    .with_operation("Operator::append_with")
+                    .with_context("service", self.info().scheme().into_static())
+                    .with_context("path", &path),
+            );
+        }
+
+        let bs = bs.into();
+        let (_, mut a) = self.inner().append(&path, args).await?;
+        a.append(bs).await?;
+        a.close().await?;
+
+        Ok(())
+    }
+
     /// Delete the given path.
     ///
     /// # Notes
     ///
     /// - Deleting a file that does not exist won't return errors.
     ///
     /// # Examples
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/ops.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/ops.rs`

 * *Files 9% similar despite different names*

```diff
@@ -393,14 +393,62 @@
     /// Set the content type of option
     pub fn with_cache_control(mut self, cache_control: &str) -> Self {
         self.cache_control = Some(cache_control.to_string());
         self
     }
 }
 
+/// Args for `append` operation.
+#[derive(Debug, Clone, Default)]
+pub struct OpAppend {
+    content_type: Option<String>,
+    content_disposition: Option<String>,
+    cache_control: Option<String>,
+}
+
+impl OpAppend {
+    /// Create a new `OpAppend`.
+    pub fn new() -> Self {
+        Self::default()
+    }
+
+    /// Get the content type from option
+    pub fn content_type(&self) -> Option<&str> {
+        self.content_type.as_deref()
+    }
+
+    /// Set the content type of option
+    pub fn with_content_type(mut self, content_type: &str) -> Self {
+        self.content_type = Some(content_type.to_string());
+        self
+    }
+
+    /// Get the content disposition from option
+    pub fn content_disposition(&self) -> Option<&str> {
+        self.content_disposition.as_deref()
+    }
+
+    /// Set the content disposition of option
+    pub fn with_content_disposition(mut self, content_disposition: &str) -> Self {
+        self.content_disposition = Some(content_disposition.to_string());
+        self
+    }
+
+    /// Get the cache control from option
+    pub fn cache_control(&self) -> Option<&str> {
+        self.cache_control.as_deref()
+    }
+
+    /// Set the content type of option
+    pub fn with_cache_control(mut self, cache_control: &str) -> Self {
+        self.cache_control = Some(cache_control.to_string());
+        self
+    }
+}
+
 /// Args for `copy` operation.
 #[derive(Debug, Clone, Default)]
 pub struct OpCopy {}
 
 impl OpCopy {
     /// Create a new `OpCopy`.
     pub fn new() -> Self {
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/reader.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/reader.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/scheme.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/scheme.rs`

 * *Files 2% similar despite different names*

```diff
@@ -31,28 +31,31 @@
 #[derive(Copy, Clone, Debug, PartialEq, Eq, Hash)]
 #[non_exhaustive]
 pub enum Scheme {
     /// [azblob][crate::services::Azblob]: Azure Storage Blob services.
     Azblob,
     /// [azdfs][crate::services::Azdfs]: Azure Data Lake Storage Gen2.
     Azdfs,
+    /// [cos][crate::services::Cos]: Tencent Cloud Object Storage services.
+    Cos,
     /// [dashmap][crate::services::Dashmap]: dashmap backend support.
     Dashmap,
     /// [fs][crate::services::Fs]: POSIX alike file system.
     Fs,
+    /// [ftp][crate::services::Ftp]: FTP backend.
+    Ftp,
     /// [gcs][crate::services::Gcs]: Google Cloud Storage backend.
     Gcs,
     /// [ghac][crate::services::Ghac]: GitHub Action Cache services.
     Ghac,
     /// [hdfs][crate::services::Hdfs]: Hadoop Distributed File System.
     Hdfs,
     /// [http][crate::services::Http]: HTTP backend.
     Http,
-    /// [ftp][crate::services::Ftp]: FTP backend.
-    Ftp,
+
     /// [ipmfs][crate::services::Ipfs]: IPFS HTTP Gateway
     Ipfs,
     /// [ipmfs][crate::services::Ipmfs]: IPFS mutable file system
     Ipmfs,
     /// [memcached][crate::services::Memcached]: Memcached service support.
     Memcached,
     /// [memory][crate::services::Memory]: In memory backend support.
@@ -75,15 +78,15 @@
     S3,
     /// [sftp][crate::services::Sftp]: SFTP services
     Sftp,
     /// [sled][crate::services::Sled]: Sled services
     Sled,
     /// [Supabase][crate::services::Supabase]: Supabase storage service
     Supabase,
-    /// [Vercel Artifacts][crate::services::vercel_artifacts]: Vercel Artifacts service, as known as Vercel Remote Caching.
+    /// [Vercel Artifacts][crate::services::VercelArtifacts]: Vercel Artifacts service, as known as Vercel Remote Caching.
     VercelArtifacts,
     /// [wasabi][crate::services::Wasabi]: Wasabi service
     Wasabi,
     /// [webdav][crate::services::Webdav]: WebDAV support.
     Webdav,
     /// [webhdfs][crate::services::Webhdfs]: WebHDFS RESTful API Services
     Webhdfs,
@@ -119,14 +122,15 @@
     type Err = Error;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         let s = s.to_lowercase();
         match s.as_str() {
             "azblob" => Ok(Scheme::Azblob),
             "azdfs" => Ok(Scheme::Azdfs),
+            "cos" => Ok(Scheme::Cos),
             "dashmap" => Ok(Scheme::Dashmap),
             "fs" => Ok(Scheme::Fs),
             "gcs" => Ok(Scheme::Gcs),
             "ghac" => Ok(Scheme::Ghac),
             "hdfs" => Ok(Scheme::Hdfs),
             "http" | "https" => Ok(Scheme::Http),
             "ftp" | "ftps" => Ok(Scheme::Ftp),
@@ -151,14 +155,15 @@
 }
 
 impl From<Scheme> for &'static str {
     fn from(v: Scheme) -> Self {
         match v {
             Scheme::Azblob => "azblob",
             Scheme::Azdfs => "azdfs",
+            Scheme::Cos => "cos",
             Scheme::Dashmap => "dashmap",
             Scheme::Fs => "fs",
             Scheme::Gcs => "gcs",
             Scheme::Ghac => "ghac",
             Scheme::Hdfs => "hdfs",
             Scheme::Http => "http",
             Scheme::Ftp => "ftp",
```

### Comparing `opendal-0.34.0/local_dependencies/opendal/src/types/writer.rs` & `opendal-0.35.0/local_dependencies/opendal/src/types/writer.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/Cargo.toml` & `opendal-0.35.0/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 
 authors= ["OpenDAL Contributors <dev@opendal.apache.org>"]
 edition= "2021"
 homepage= "https://opendal.apache.org/"
 license= "Apache-2.0"
 repository= "https://github.com/apache/incubator-opendal"
 rust-version= "1.65"
-version= "0.34.0"
+version= "0.35.0"
 
 [lib]
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
-chrono = { version = "0.4.24", default-features = false, features = ["std"] }
 futures = "0.3.28"
 opendal.path = "local_dependencies/opendal"
-pyo3 = { version = "0.18", features = ["chrono"] }
+pyo3 = { version = "0.18", features = ["abi3-py37"] }
 pyo3-asyncio = { version = "0.18", features = ["tokio-runtime"] }
 tokio = "1"
```

### Comparing `opendal-0.34.0/.gitignore` & `opendal-0.35.0/.gitignore`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/CONTRIBUTING.md` & `opendal-0.35.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/README.md` & `opendal-0.35.0/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/benchmark/README.md` & `opendal-0.35.0/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/benchmark/async_opendal_benchmark.py` & `opendal-0.35.0/benchmark/async_opendal_benchmark.py`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/benchmark/async_origin_s3_benchmark_with_gevent.py` & `opendal-0.35.0/benchmark/async_origin_s3_benchmark_with_gevent.py`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/examples/object.ipynb` & `opendal-0.35.0/examples/object.ipynb`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/pyproject.toml` & `opendal-0.35.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/python/opendal/__init__.py` & `opendal-0.35.0/python/opendal/__init__.py`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/python/opendal/__init__.pyi` & `opendal-0.35.0/python/opendal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/src/asyncio.rs` & `opendal-0.35.0/src/asyncio.rs`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/src/layers.rs` & `opendal-0.35.0/src/layers.rs`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 // Unless required by applicable law or agreed to in writing,
 // software distributed under the License is distributed on an
 // "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 // KIND, either express or implied.  See the License for the
 // specific language governing permissions and limitations
 // under the License.
 
+use std::time::Duration;
+
 use ::opendal as od;
-use chrono::Duration;
-use pyo3::exceptions::PyOverflowError;
 use pyo3::prelude::*;
 
 #[derive(FromPyObject)]
 pub enum Layer {
     ConcurrentLimit(ConcurrentLimitLayer),
     ImmutableIndex(ImmutableIndexLayer),
     Retry(RetryLayer),
@@ -69,40 +69,32 @@
         max_delay = None,
         min_delay = None
     ))]
     fn new(
         max_times: Option<usize>,
         factor: Option<f32>,
         jitter: bool,
-        max_delay: Option<Duration>,
-        min_delay: Option<Duration>,
+        max_delay: Option<f64>,
+        min_delay: Option<f64>,
     ) -> PyResult<Self> {
         let mut retry = od::layers::RetryLayer::default();
         if let Some(max_times) = max_times {
             retry = retry.with_max_times(max_times);
         }
         if let Some(factor) = factor {
             retry = retry.with_factor(factor);
         }
         if jitter {
             retry = retry.with_jitter();
         }
         if let Some(max_delay) = max_delay {
-            retry = retry.with_max_delay(
-                max_delay
-                    .to_std()
-                    .map_err(|err| PyOverflowError::new_err(err.to_string()))?,
-            );
+            retry = retry.with_max_delay(Duration::from_micros((max_delay * 1000000.0) as u64));
         }
         if let Some(min_delay) = min_delay {
-            retry = retry.with_min_delay(
-                min_delay
-                    .to_std()
-                    .map_err(|err| PyOverflowError::new_err(err.to_string()))?,
-            );
+            retry = retry.with_min_delay(Duration::from_micros((min_delay * 1000000.0) as u64));
         }
         Ok(Self(retry))
     }
 }
 
 pub fn create_submodule(py: Python) -> PyResult<&PyModule> {
     let submod = PyModule::new(py, "layers")?;
```

### Comparing `opendal-0.34.0/src/lib.rs` & `opendal-0.35.0/src/lib.rs`

 * *Files 16% similar despite different names*

```diff
@@ -58,60 +58,15 @@
 }
 
 fn build_operator(
     scheme: od::Scheme,
     map: HashMap<String, String>,
     layers: Vec<layers::Layer>,
 ) -> PyResult<od::Operator> {
-    use od::services::*;
-
-    let op = match scheme {
-        od::Scheme::Azblob => od::Operator::from_map::<Azblob>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Azdfs => od::Operator::from_map::<Azdfs>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Fs => od::Operator::from_map::<Fs>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Gcs => od::Operator::from_map::<Gcs>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Ghac => od::Operator::from_map::<Ghac>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Http => od::Operator::from_map::<Http>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Ipmfs => od::Operator::from_map::<Ipmfs>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Memory => od::Operator::from_map::<Memory>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Obs => od::Operator::from_map::<Obs>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Oss => od::Operator::from_map::<Oss>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::S3 => od::Operator::from_map::<S3>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Webdav => od::Operator::from_map::<Webdav>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        od::Scheme::Webhdfs => od::Operator::from_map::<Webhdfs>(map)
-            .map_err(format_pyerr)?
-            .finish(),
-        _ => Err(PyNotImplementedError::new_err(format!(
-            "unsupported scheme `{scheme}`"
-        )))?,
-    };
+    let op = od::Operator::via_map(scheme, map).map_err(format_pyerr)?;
 
     add_layers(op, layers)
 }
 
 /// `Operator` is the entry for all public blocking APIs
 ///
 /// Create a new blocking `Operator` with the given `scheme` and options(`**kwargs`).
```

### Comparing `opendal-0.34.0/tests/binding.feature` & `opendal-0.35.0/tests/binding.feature`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/tests/steps/binding.py` & `opendal-0.35.0/tests/steps/binding.py`

 * *Files identical despite different names*

### Comparing `opendal-0.34.0/Cargo.lock` & `opendal-0.35.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,17 @@
 dependencies = [
  "anstyle 1.0.0",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
@@ -258,15 +258,15 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "async-task"
 version = "4.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ecc7ab41815b3c653ccd2978ec3255c81349336702dfdf62ee6f7069b12a3aae"
@@ -288,15 +288,15 @@
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "atomic-waker"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "debc29dde2e69f9e47506b525f639ed42300fc014a3e007832592448fa8e4599"
@@ -1004,15 +1004,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "edc52e2eb08915cb12596d29d55f0b5384f00d697a646dbd269b6ecb0fbd9d31"
@@ -1021,15 +1021,15 @@
 name = "cxxbridge-macro"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "631569015d0d8d54e6c241733f944042623ab6df7bc3be7466874b05fcdb1c5f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
@@ -1099,17 +1099,17 @@
 name = "deadpool-runtime"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eaa37046cc0f6c3cc6090fbdbf73ef0b8ef4cfcc37f6befc0020f63e8cf121e1"
 
 [[package]]
 name = "der"
-version = "0.6.1"
+version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1a467a65c5e759bce6e65eaf91cc29f466cdc57cb65777bd646872a8a1fd4de"
+checksum = "56acb310e15652100da43d130af8d97b509e95af61aab1c5a7939ef24337ee17"
 dependencies = [
  "const-oid",
  "pem-rfc7468",
  "zeroize",
 ]
 
 [[package]]
@@ -1154,19 +1154,19 @@
 checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
 dependencies = [
  "dirs-sys 0.3.7",
 ]
 
 [[package]]
 name = "dirs"
-version = "5.0.0"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dece029acd3353e3a58ac2e3eb3c8d6c35827a892edc6cc4138ef9c33df46ecd"
+checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
 dependencies = [
- "dirs-sys 0.4.0",
+ "dirs-sys 0.4.1",
 ]
 
 [[package]]
 name = "dirs-sys"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
@@ -1174,21 +1174,22 @@
  "libc",
  "redox_users",
  "winapi",
 ]
 
 [[package]]
 name = "dirs-sys"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04414300db88f70d74c5ff54e50f9e1d1737d9a5b90f53fcf2e95ca2a9ab554b"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
 dependencies = [
  "libc",
+ "option-ext",
  "redox_users",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "dlv-list"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d529fd73d344663edfd598ccb3f344e46034db51ebd103518eae34338248ad73"
@@ -1421,15 +1422,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -2527,21 +2528,21 @@
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "oay"
-version = "0.34.0"
+version = "0.35.0"
 dependencies = [
  "anyhow",
  "axum",
  "chrono",
  "clap 4.2.5",
- "dirs 5.0.0",
+ "dirs 5.0.1",
  "futures",
  "opendal",
  "quick-xml 0.27.1",
  "serde",
  "tokio",
  "toml 0.7.3",
  "tower",
@@ -2570,32 +2571,32 @@
  "tracing",
  "url",
  "walkdir",
 ]
 
 [[package]]
 name = "object_store_opendal"
-version = "0.34.0"
+version = "0.35.0"
 dependencies = [
  "async-trait",
  "bytes",
  "futures",
  "object_store",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "oli"
-version = "0.34.0"
+version = "0.35.0"
 dependencies = [
  "anyhow",
  "assert_cmd",
  "clap 4.2.5",
- "dirs 5.0.0",
+ "dirs 5.0.1",
  "env_logger",
  "futures",
  "log",
  "opendal",
  "predicates 2.1.5",
  "serde",
  "tokio",
@@ -2613,27 +2614,28 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "opendal"
-version = "0.34.0"
+version = "0.35.0"
 dependencies = [
  "anyhow",
  "async-compat",
  "async-tls",
  "async-trait",
  "backon",
  "base64 0.21.0",
  "bb8",
  "bytes",
  "chrono",
  "criterion",
  "dashmap",
+ "dirs 5.0.1",
  "dotenvy",
  "flagset",
  "futures",
  "hdrs",
  "http",
  "hyper",
  "lazy-regex",
@@ -2644,15 +2646,14 @@
  "minitrace",
  "moka",
  "once_cell",
  "openssh",
  "openssh-sftp-client",
  "opentelemetry 0.19.0",
  "opentelemetry-jaeger",
- "owning_ref",
  "parking_lot 0.12.1",
  "paste",
  "percent-encoding",
  "pin-project",
  "pretty_assertions",
  "prometheus",
  "prost",
@@ -2685,37 +2686,37 @@
  "opendal",
 ]
 
 [[package]]
 name = "opendal-java"
 version = "0.1.0"
 dependencies = [
+ "anyhow",
  "jni",
  "num_cpus",
  "once_cell",
  "opendal",
  "tokio",
 ]
 
 [[package]]
 name = "opendal-nodejs"
-version = "0.34.0"
+version = "0.35.0"
 dependencies = [
  "futures",
  "napi",
  "napi-build",
  "napi-derive",
  "opendal",
 ]
 
 [[package]]
 name = "opendal-python"
-version = "0.34.0"
+version = "0.35.0"
 dependencies = [
- "chrono",
  "futures",
  "opendal",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
 ]
 
@@ -2743,53 +2744,58 @@
  "thiserror",
  "tokio",
  "tokio-pipe",
 ]
 
 [[package]]
 name = "openssh-sftp-client"
-version = "0.12.2"
+version = "0.13.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4fa8e5f26e549bd266d9bcd9e5b4fd344729985ef1a7f5ac3e51f3f96a4a620"
+checksum = "866d0eab409a2fcb6b8c3838fdbf10d7399d486548c19179a80f1c1142e93348"
 dependencies = [
  "bytes",
  "derive_destructure2",
+ "futures-core",
  "once_cell",
+ "openssh",
  "openssh-sftp-client-lowlevel",
  "openssh-sftp-error",
+ "pin-project",
  "scopeguard",
  "tokio",
  "tokio-io-utility",
  "tokio-util",
+ "tracing",
 ]
 
 [[package]]
 name = "openssh-sftp-client-lowlevel"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406bf41d8372365497d5645e802a8dfe22008b8183edbe6c79e4b75614431daa"
+checksum = "f4975d0a824e82d4f61e3edf870254ce97bd7f8154751d2afdd97c7f43e57dff"
 dependencies = [
  "awaitable",
  "bytes",
  "concurrent_arena",
  "derive_destructure2",
  "openssh-sftp-error",
  "openssh-sftp-protocol",
  "pin-project",
  "tokio",
  "tokio-io-utility",
 ]
 
 [[package]]
 name = "openssh-sftp-error"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d836b428ead150165d1178ed0aa672791c13b3ae9616ea1e34d13730a2cb486"
+checksum = "f4c3356e914b8006417188efd534105d5bcb230b4a9fd67782a6b4a4e15fa006"
 dependencies = [
  "awaitable-error",
+ "openssh",
  "openssh-sftp-protocol-error",
  "ssh_format_error",
  "thiserror",
  "tokio",
 ]
 
 [[package]]
@@ -2957,14 +2963,20 @@
  "opentelemetry_api",
  "percent-encoding",
  "rand 0.8.5",
  "thiserror",
 ]
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "ordered-float"
 version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7940cf2ca942593318d07fcf2596cdca60a85c9e7fab408a5e21a4f9dcd40d87"
 dependencies = [
  "num-traits",
 ]
@@ -2997,23 +3009,14 @@
 [[package]]
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
-name = "owning_ref"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ff55baddef9e4ad00f88b6c743a2a8062d4c6ade126c2a528644b8e444d52ce"
-dependencies = [
- "stable_deref_trait",
-]
-
-[[package]]
 name = "parking"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "427c3892f9e783d91cc128285287e70a59e206ca452770ece88a76f7a3eddd72"
 
 [[package]]
 name = "parking_lot"
@@ -3082,17 +3085,17 @@
 checksum = "a8835c273a76a90455d7344889b0964598e3316e2a79ede8e36f16bdcf2228b8"
 dependencies = [
  "base64 0.13.1",
 ]
 
 [[package]]
 name = "pem-rfc7468"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24d159833a9105500e0398934e205e0773f0b27529557134ecfc51c27646adac"
+checksum = "88b39c9bfcfc231068454382784bb460aae594343fb030d46e9f50a645418412"
 dependencies = [
  "base64ct",
 ]
 
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
@@ -3129,29 +3132,28 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkcs1"
-version = "0.4.1"
+version = "0.7.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eff33bdbdfc54cc98a2eca766ebdec3e1b8fb7387523d5c9c9a2891da856f719"
+checksum = "c8ffb9f10fa047879315e6625af03c164b16962a5368d724ed16323b68ace47f"
 dependencies = [
  "der",
  "pkcs8",
  "spki",
- "zeroize",
 ]
 
 [[package]]
 name = "pkcs8"
-version = "0.9.0"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9eca2c590a5f85da82668fa685c09ce2888b9430e83299debf1f34b65fd4a4ba"
+checksum = "f950b2377845cebe5cf8b5165cb3cc1a5e0fa5cfa3e1f7f55707d8fd82e0a7b7"
 dependencies = [
  "der",
  "spki",
 ]
 
 [[package]]
 name = "pkg-config"
@@ -3297,17 +3299,17 @@
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "procfs"
 version = "0.14.2"
@@ -3381,15 +3383,14 @@
 [[package]]
 name = "pyo3"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
- "chrono",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
@@ -3710,17 +3711,17 @@
 name = "regex-syntax"
 version = "0.6.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
 
 [[package]]
 name = "reqsign"
-version = "0.10.1"
+version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d36dae58fbc1db90e1cf14ca8fabcba92b7aa3c282d5e46bcdf16b9c28ab04c"
+checksum = "b04f5fccb94d61c154f0d8520ec42e79afdc145f4b1a392faa269874995fda66"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.0",
  "chrono",
  "form_urlencoded",
  "hex",
@@ -3827,28 +3828,30 @@
 dependencies = [
  "libc",
  "librocksdb-sys",
 ]
 
 [[package]]
 name = "rsa"
-version = "0.8.2"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55a77d189da1fee555ad95b7e50e7457d91c0e089ec68ca69ad2989413bbdab4"
+checksum = "6ab43bb47d23c1a631b4b680199a45255dce26fa9ab2fa902581f624ff13e6a8"
 dependencies = [
  "byteorder",
+ "const-oid",
  "digest",
  "num-bigint-dig",
  "num-integer",
  "num-iter",
  "num-traits",
  "pkcs1",
  "pkcs8",
  "rand_core 0.6.4",
  "signature",
+ "spki",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-ini"
 version = "0.19.0"
@@ -4050,15 +4053,15 @@
 name = "serde_derive"
 version = "1.0.158"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e801c1712f48475582b7696ac71e0ca34ebb30e09338425384269d9717c62cad"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
@@ -4292,17 +4295,17 @@
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "spki"
-version = "0.6.0"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67cf02bbac7a337dc36e4f5a693db6c21e7863f45070f7064577eb4367a3212b"
+checksum = "9d1e996ef02c474957d681f1b05213dfb0abab947b446a62d37770b23500184a"
 dependencies = [
  "base64ct",
  "der",
 ]
 
 [[package]]
 name = "ssh_format"
@@ -4366,17 +4369,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.12"
+version = "2.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "79d9531f94112cfc3e4c8f5f02cb2b58f72c97b7efd85f70203cc6d8efda5927"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -4450,15 +4453,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -4559,50 +4562,50 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "0aa32867d44e6f2ce3385e89dceb990188b8bb0fb25b0cf576647a6f98ac5105"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-io-utility"
 version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d672654d175710e52c7c41f6aec77c62b3c0954e2a7ebce9049d1e94ed7c263"
 dependencies = [
  "bytes",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.12",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
```

### Comparing `opendal-0.34.0/PKG-INFO` & `opendal-0.35.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opendal
-Version: 0.34.0
+Version: 0.35.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: gevent ; extra == 'benchmark'
 Requires-Dist: greenify ; extra == 'benchmark'
 Requires-Dist: greenlet ; extra == 'benchmark'
 Requires-Dist: boto3 ; extra == 'benchmark'
```

