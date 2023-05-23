# Comparing `tmp/moralis-0.1.8.tar.gz` & `tmp/moralis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moralis-0.1.8.tar", last modified: Tue Dec 13 19:33:36 2022, max compression
+gzip compressed data, was "moralis-0.1.9.tar", last modified: Tue Dec 13 20:15:54 2022, max compression
```

## Comparing `moralis-0.1.8.tar` & `moralis-0.1.9.tar`

### file list

```diff
@@ -1,733 +1,737 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.422632 moralis-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-13 19:33:20.000000 moralis-0.1.8/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2022-12-13 19:33:36.422632 moralis-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2022-12-13 19:33:20.000000 moralis-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 19:33:36.422632 moralis-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-13 19:33:35.000000 moralis-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.326632 moralis-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.330632 moralis-0.1.8/src/moralis/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-13 19:33:35.000000 moralis-0.1.8/src/moralis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.330632 moralis-0.1.8/src/moralis/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.330632 moralis-0.1.8/src/moralis/auth/challenge/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/challenge/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/challenge/challenge.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/challenge/request_challenge_evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/challenge/request_challenge_solana.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/challenge/verify_challenge_evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/challenge/verify_challenge_solana.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/auth/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.330632 moralis-0.1.8/src/moralis/evm_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.330632 moralis-0.1.8/src/moralis/evm_api/balance/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/balance/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/balance/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/balance/get_native_balance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.334632 moralis-0.1.8/src/moralis/evm_api/block/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/block/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/block/block.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/block/get_date_to_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.334632 moralis-0.1.8/src/moralis/evm_api/defi/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/defi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/defi/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/defi/defi.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/defi/get_pair_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/defi/get_pair_reserves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.334632 moralis-0.1.8/src/moralis/evm_api/events/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/events/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/events/get_contract_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/events/get_contract_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/evm_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.334632 moralis-0.1.8/src/moralis/evm_api/ipfs/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/ipfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/ipfs/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/ipfs/ipfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/ipfs/upload_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.338632 moralis-0.1.8/src/moralis/evm_api/nft/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_contract_nfts.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_multiple_nfts.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_contract_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_lowest_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_owners.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_token_id_owners.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_trades.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_transfers_by_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_nft_transfers_from_to_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_wallet_nft_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_wallet_nft_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/get_wallet_nfts.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/re_sync_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/search_nfts.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/nft/sync_nft_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.338632 moralis-0.1.8/src/moralis/evm_api/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/resolve/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/resolve/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/resolve/resolve_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/resolve/resolve_domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.338632 moralis-0.1.8/src/moralis/evm_api/token/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/get_token_allowance.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/get_token_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/get_token_metadata_by_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/get_token_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/get_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/get_wallet_token_balances.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/get_wallet_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/token/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.338632 moralis-0.1.8/src/moralis/evm_api/transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/transaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/transaction/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/transaction/get_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/transaction/get_wallet_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/transaction/get_wallet_transactions_verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/transaction/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.338632 moralis-0.1.8/src/moralis/evm_api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/utils/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/utils/endpoint_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/utils/run_contract_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/evm_api/utils/web3_api_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.338632 moralis-0.1.8/src/moralis/sol_api/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.342632 moralis-0.1.8/src/moralis/sol_api/account/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/account/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/account/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/account/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/account/get_nfts.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/account/get_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/account/get_spl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.342632 moralis-0.1.8/src/moralis/sol_api/nft/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/nft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/nft/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/nft/get_nft_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/nft/nft.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/sol_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.342632 moralis-0.1.8/src/moralis/sol_api/token/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/token/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/token/get_token_price.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/token/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/sol_api/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.342632 moralis-0.1.8/src/moralis/streams/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.342632 moralis-0.1.8/src/moralis/streams/evm/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/add_address_to_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/create_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/delete_address_from_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/delete_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/get_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/get_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/get_streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/update_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/evm/update_stream_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.346632 moralis-0.1.8/src/moralis/streams/history/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/history/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/history/get_history.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/history/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/history/replay_history.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.346632 moralis-0.1.8/src/moralis/streams/project/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/project/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/project/get_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/project/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/project/set_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.346632 moralis-0.1.8/src/moralis/streams/stats/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/stats/api_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/stats/get_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/stats/get_stats_by_stream_id.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/stats/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-13 19:33:20.000000 moralis-0.1.8/src/moralis/streams/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.330632 moralis-0.1.8/src/moralis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2022-12-13 19:33:36.000000 moralis-0.1.8/src/moralis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30618 2022-12-13 19:33:36.000000 moralis-0.1.8/src/moralis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 19:33:36.000000 moralis-0.1.8/src/moralis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-13 19:33:36.000000 moralis-0.1.8/src/moralis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-13 19:33:36.000000 moralis-0.1.8/src/moralis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.346632 moralis-0.1.8/src/openapi_auth/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58553 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.346632 moralis-0.1.8/src/openapi_auth/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.346632 moralis-0.1.8/src/openapi_auth/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/paths/challenge_request_evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/paths/challenge_request_solana.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/paths/challenge_verify_evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/paths/challenge_verify_solana.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.346632 moralis-0.1.8/src/openapi_auth/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/apis/tags/challenge_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16515 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/model/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/evm_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/evm_challenge_response_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/evm_complete_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/evm_complete_challenge_response_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/solana_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/solana_challenge_response_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/solana_complete_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/model/solana_complete_challenge_response_dto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/paths/challenge_request_evm/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_request_evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_request_evm/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/paths/challenge_request_solana/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_request_solana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_request_solana/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/paths/challenge_verify_evm/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_verify_evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_verify_evm/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/paths/challenge_verify_solana/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_verify_solana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11815 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/paths/challenge_verify_solana/post.py
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2022-12-13 19:33:20.000000 moralis-0.1.8/src/openapi_auth/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    97622 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_auth/test/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_challenge_response_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_complete_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_complete_challenge_response_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_challenge_response_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_complete_challenge_request_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_complete_challenge_response_dto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.350632 moralis-0.1.8/src/openapi_evm_api/
--rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58618 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.354632 moralis-0.1.8/src/openapi_evm_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.358632 moralis-0.1.8/src/openapi_evm_api/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_erc20_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_nft_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_nft_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/address_verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/block_block_number_or_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/block_block_number_or_hash_nft_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/date_to_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/erc20_address_allowance.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/erc20_address_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/erc20_address_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/erc20_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/erc20_metadata_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/info_endpoint_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/ipfs_upload_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_lowestprice.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_owners.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_token_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_token_id_metadata_resync.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_token_id_owners.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_token_id_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_trades.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_address_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_get_multiple_nfts.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/nft_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/pair_address_reserves.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/resolve_address_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/resolve_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/token0_address_token1_address_pair_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/transaction_transaction_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/paths/web3_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.358632 moralis-0.1.8/src/openapi_evm_api/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/balance_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/block_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/defi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/events_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/ipfs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/nft_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/resolve_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/token_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/apis/tags/utils_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16597 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/block_date.py
--rw-r--r--   0 runner    (1001) docker     (123)    19567 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/block_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/chain_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/endpoint_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/ens.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/erc20_allowance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/erc20_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/erc20_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/erc20_token_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/erc20_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/erc20_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3627 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/erc721_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/get_multiple_nfts_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/historical_nft_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/ipfs_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/ipfs_file_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/log_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/log_event_by_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/metadata_resync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/native_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/native_erc20_price.py
--rw-r--r--   0 runner    (1001) docker     (123)    11497 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft.py
--rw-r--r--   0 runner    (1001) docker     (123)     5515 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_contract_metadata_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_metadata_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_owner_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_transfer_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/nft_wallet_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/normalized_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/normalized_metadata_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    19827 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/reserves_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/reserves_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/run_contract_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/token_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/trade.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/trade_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/transaction_collection_verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/model/web3version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13971 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_balance/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_balance/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_erc20/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_erc20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_erc20/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_erc20_transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_erc20_transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14019 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_erc20_transfers/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_events/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23276 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_events/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_function/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16490 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_function/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_logs/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_logs/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_nft/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_nft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14405 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_nft/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_nft_collections/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_nft_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_nft_collections/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_nft_transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_nft_transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14623 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_nft_transfers/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/address_verbose/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_verbose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/address_verbose/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11886 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.366632 moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12753 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/date_to_block/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/date_to_block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10199 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/date_to_block/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_allowance/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_allowance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_allowance/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_price/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_price/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_transfers/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata_symbols/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata_symbols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata_symbols/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/info_endpoint_weights/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/info_endpoint_weights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/info_endpoint_weights/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/ipfs_upload_folder/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/ipfs_upload_folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13228 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/ipfs_upload_folder/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14247 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_lowestprice/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_lowestprice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_lowestprice/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12028 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_metadata/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_owners/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_owners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13484 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_owners/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_sync/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13112 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.370632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_owners/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_owners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_owners/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_transfers/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_trades/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_trades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_trades/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_address_transfers/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/nft_get_multiple_nfts/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_get_multiple_nfts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14571 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_get_multiple_nfts/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/nft_search/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_search/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/nft_transfers/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/nft_transfers/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/pair_address_reserves/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/pair_address_reserves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14700 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/pair_address_reserves/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/resolve_address_reverse/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/resolve_address_reverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/resolve_address_reverse/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/resolve_domain/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/resolve_domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/resolve_domain/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/transaction_transaction_hash/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/transaction_transaction_hash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/transaction_transaction_hash/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/paths/web3_version/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/web3_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/paths/web3_version/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    97681 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.374632 moralis-0.1.8/src/openapi_evm_api/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.382632 moralis-0.1.8/src/openapi_evm_api/test/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_block_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_block_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_chain_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_endpoint_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_ens.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_allowance.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_token_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc721_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_get_multiple_nfts_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_historical_nft_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_ipfs_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_ipfs_file_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log_event_by_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_metadata_resync.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_native_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_native_erc20_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_contract_metadata_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_metadata_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_owner_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_transfer_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_wallet_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_normalized_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_normalized_metadata_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_reserves_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_reserves_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_run_contract_dto.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_token_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_trade.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_trade_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_transaction_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_transaction_collection_verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_evm_api/test/test_models/test_web3version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.382632 moralis-0.1.8/src/openapi_sol_api/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58533 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.382632 moralis-0.1.8/src/openapi_sol_api/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.382632 moralis-0.1.8/src/openapi_sol_api/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/paths/account_network_address_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/paths/account_network_address_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/paths/account_network_address_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/paths/account_network_address_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/paths/nft_network_address_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/paths/token_network_address_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.382632 moralis-0.1.8/src/openapi_sol_api/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/tags/account_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/tags/nft_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/apis/tags/token_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16506 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.386632 moralis-0.1.8/src/openapi_sol_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/metaplex_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/native_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/nft_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/spl_native_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/spl_token_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/spl_token_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/model/splnft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.386632 moralis-0.1.8/src/openapi_sol_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.386632 moralis-0.1.8/src/openapi_sol_api/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.386632 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_balance/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_balance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_balance/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.386632 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_nft/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_nft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_nft/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.386632 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_portfolio/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_portfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_portfolio/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.386632 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_tokens/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_tokens/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.390632 moralis-0.1.8/src/openapi_sol_api/paths/nft_network_address_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/nft_network_address_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10852 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/nft_network_address_metadata/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.390632 moralis-0.1.8/src/openapi_sol_api/paths/token_network_address_price/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/token_network_address_price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10733 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/paths/token_network_address_price/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    10487 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    97596 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.390632 moralis-0.1.8/src/openapi_sol_api/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.390632 moralis-0.1.8/src/openapi_sol_api/test/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_metaplex_nft.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_native_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_nft_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_spl_native_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_spl_token_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_spl_token_price.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_sol_api/test/test_models/test_splnft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.394632 moralis-0.1.8/src/openapi_streams/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58561 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.394632 moralis-0.1.8/src/openapi_streams/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.394632 moralis-0.1.8/src/openapi_streams/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/history_replay_stream_id_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/stats_stream_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/streams_evm.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/streams_evm_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/streams_evm_id_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/paths/streams_evm_id_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.394632 moralis-0.1.8/src/openapi_streams/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/tags/evm_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/tags/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/tags/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/apis/tags/stats_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4486 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.402632 moralis-0.1.8/src/openapi_streams/model/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/abi_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/abi_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/abi_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/addresses_types_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/addresses_types_addresses_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/addresses_types_addresses_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/addresses_types_addresses_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/addresses_types_delete_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/addresses_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/advanced_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/history_types_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/history_types_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/history_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/internal_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/partial_streams_types_streams_model_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/settings_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/settings_types_settings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/stream_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13570 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_types_streams_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11751 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_types_streams_model_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_types_streams_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_types_streams_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/streams_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21422 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/usagestats_types_usage_stats_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4445 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/webhook_types_i_tiny_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/model/webhook_types_i_webhook_un_parsed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.402632 moralis-0.1.8/src/openapi_streams/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.406632 moralis-0.1.8/src/openapi_streams/paths/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.406632 moralis-0.1.8/src/openapi_streams/paths/history/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10520 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/history/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.406632 moralis-0.1.8/src/openapi_streams/paths/history_replay_stream_id_id/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/history_replay_stream_id_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/history_replay_stream_id_id/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.406632 moralis-0.1.8/src/openapi_streams/paths/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/settings/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/settings/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.406632 moralis-0.1.8/src/openapi_streams/paths/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/stats/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.406632 moralis-0.1.8/src/openapi_streams/paths/stats_stream_id/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/stats_stream_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9919 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/stats_stream_id/get.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.406632 moralis-0.1.8/src/openapi_streams/paths/streams_evm/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10184 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm/put.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.410632 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    13891 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.410632 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14073 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)    12250 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/get.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/post.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.410632 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_status/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_status/post.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    97624 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.410632 moralis-0.1.8/src/openapi_streams/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:36.422632 moralis-0.1.8/src/openapi_streams/test/test_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_abi_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_abi_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_abi_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_addresses_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_addresses_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_addresses_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_delete_address_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_advanced_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_history_types_history_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_history_types_history_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_history_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_internal_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_partial_streams_types_streams_model_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_settings_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_settings_types_settings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_stream_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_model_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_status_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_usagestats_types_usage_stats_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_webhook_types_i_tiny_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2022-12-13 19:33:21.000000 moralis-0.1.8/src/openapi_streams/test/test_models/test_webhook_types_i_webhook_un_parsed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.911042 moralis-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-13 20:15:40.000000 moralis-0.1.9/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2022-12-13 20:15:54.907042 moralis-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2022-12-13 20:15:40.000000 moralis-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 20:15:54.911042 moralis-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2022-12-13 20:15:54.000000 moralis-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.831042 moralis-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.835042 moralis-0.1.9/src/moralis/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.835042 moralis-0.1.9/src/moralis/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.835042 moralis-0.1.9/src/moralis/auth/challenge/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/challenge/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/challenge/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/challenge/request_challenge_evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/challenge/request_challenge_solana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/challenge/verify_challenge_evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/challenge/verify_challenge_solana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/auth/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis/auth/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.835042 moralis-0.1.9/src/moralis/evm_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.839042 moralis-0.1.9/src/moralis/evm_api/balance/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/balance/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/balance/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/balance/get_native_balance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.839042 moralis-0.1.9/src/moralis/evm_api/block/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/block/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/block/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/block/get_date_to_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.839042 moralis-0.1.9/src/moralis/evm_api/defi/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/defi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/defi/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/defi/defi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/defi/get_pair_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/defi/get_pair_reserves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.839042 moralis-0.1.9/src/moralis/evm_api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/events/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/events/get_contract_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/events/get_contract_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/evm_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.839042 moralis-0.1.9/src/moralis/evm_api/ipfs/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/ipfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/ipfs/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/ipfs/ipfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/ipfs/upload_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.843042 moralis-0.1.9/src/moralis/evm_api/nft/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_contract_nfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_multiple_nfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_contract_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_lowest_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_token_id_owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_transfers_by_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_nft_transfers_from_to_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_wallet_nft_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_wallet_nft_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/get_wallet_nfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/re_sync_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/search_nfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/nft/sync_nft_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.843042 moralis-0.1.9/src/moralis/evm_api/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/resolve/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/resolve/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/resolve/resolve_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/resolve/resolve_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.843042 moralis-0.1.9/src/moralis/evm_api/token/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/get_token_allowance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/get_token_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/get_token_metadata_by_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/get_token_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/get_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/get_wallet_token_balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/get_wallet_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/token/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.847042 moralis-0.1.9/src/moralis/evm_api/transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/transaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/transaction/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/transaction/get_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/transaction/get_wallet_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/transaction/get_wallet_transactions_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/transaction/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.847042 moralis-0.1.9/src/moralis/evm_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/utils/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/utils/endpoint_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/utils/run_contract_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/evm_api/utils/web3_api_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis/evm_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.847042 moralis-0.1.9/src/moralis/sol_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.847042 moralis-0.1.9/src/moralis/sol_api/account/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/account/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/account/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/account/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/account/get_nfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/account/get_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/account/get_spl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.847042 moralis-0.1.9/src/moralis/sol_api/nft/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/nft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/nft/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/nft/get_nft_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/nft/nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/sol_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.847042 moralis-0.1.9/src/moralis/sol_api/token/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/token/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/token/get_token_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/token/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/sol_api/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis/sol_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.847042 moralis-0.1.9/src/moralis/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.851042 moralis-0.1.9/src/moralis/streams/evm/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/add_address_to_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/create_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/delete_address_from_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/delete_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/get_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/get_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/get_streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/update_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/evm/update_stream_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.851042 moralis-0.1.9/src/moralis/streams/history/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/history/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/history/get_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/history/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/history/replay_history.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.851042 moralis-0.1.9/src/moralis/streams/project/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/project/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/project/get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/project/set_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.851042 moralis-0.1.9/src/moralis/streams/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/stats/api_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/stats/get_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/stats/get_stats_by_stream_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/stats/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2022-12-13 20:15:40.000000 moralis-0.1.9/src/moralis/streams/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis/streams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.835042 moralis-0.1.9/src/moralis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30739 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-13 20:15:54.000000 moralis-0.1.9/src/moralis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.851042 moralis-0.1.9/src/openapi_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58553 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/path_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/apis/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/paths/challenge_request_evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/paths/challenge_request_solana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/paths/challenge_verify_evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/paths/challenge_verify_solana.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/tag_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/apis/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/apis/tags/challenge_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16515 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/evm_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/evm_challenge_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/evm_complete_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/evm_complete_challenge_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/solana_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/solana_challenge_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/solana_complete_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10131 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/model/solana_complete_challenge_response_dto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/paths/challenge_request_evm/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_request_evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_request_evm/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/paths/challenge_request_solana/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_request_solana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_request_solana/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/paths/challenge_verify_evm/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_verify_evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_verify_evm/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/paths/challenge_verify_solana/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_verify_solana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/paths/challenge_verify_solana/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97622 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.855042 moralis-0.1.9/src/openapi_auth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.859042 moralis-0.1.9/src/openapi_auth/test/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_challenge_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_complete_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_complete_challenge_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_challenge_response_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_complete_challenge_request_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_complete_challenge_response_dto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.859042 moralis-0.1.9/src/openapi_evm_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58618 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.859042 moralis-0.1.9/src/openapi_evm_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/path_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.863042 moralis-0.1.9/src/openapi_evm_api/apis/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_erc20_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_nft_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_nft_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/address_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/block_block_number_or_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/block_block_number_or_hash_nft_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/date_to_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/erc20_address_allowance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/erc20_address_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/erc20_address_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/erc20_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/erc20_metadata_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/info_endpoint_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/ipfs_upload_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_lowestprice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_token_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_token_id_metadata_resync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_token_id_owners.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_token_id_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_address_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_get_multiple_nfts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/nft_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/pair_address_reserves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/resolve_address_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/resolve_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/token0_address_token1_address_pair_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/transaction_transaction_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/paths/web3_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tag_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.867042 moralis-0.1.9/src/openapi_evm_api/apis/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/balance_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/block_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/defi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/ipfs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/nft_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/resolve_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/token_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/apis/tags/utils_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16597 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.871042 moralis-0.1.9/src/openapi_evm_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13877 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/block_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19567 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/block_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/chain_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/endpoint_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/ens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/erc20_allowance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/erc20_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/erc20_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/erc20_token_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/erc20_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/erc20_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/erc721_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/get_multiple_nfts_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/historical_nft_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/ipfs_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/ipfs_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/log_event_by_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/metadata_resync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/native_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/native_erc20_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11497 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_contract_metadata_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_metadata_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_owner_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6835 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_transfer_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/nft_wallet_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/normalized_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/normalized_metadata_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19827 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/reserves_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/reserves_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/run_contract_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/token_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5028 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/trade_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/transaction_collection_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/model/web3version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.871042 moralis-0.1.9/src/openapi_evm_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.871042 moralis-0.1.9/src/openapi_evm_api/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.871042 moralis-0.1.9/src/openapi_evm_api/paths/address/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13971 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.871042 moralis-0.1.9/src/openapi_evm_api/paths/address_balance/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_balance/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.871042 moralis-0.1.9/src/openapi_evm_api/paths/address_erc20/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_erc20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_erc20/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.871042 moralis-0.1.9/src/openapi_evm_api/paths/address_erc20_transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_erc20_transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14019 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_erc20_transfers/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/address_events/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23276 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_events/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/address_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16490 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_function/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/address_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_logs/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/address_nft/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_nft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14405 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_nft/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/address_nft_collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_nft_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_nft_collections/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/address_nft_transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_nft_transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14623 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_nft_transfers/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/address_verbose/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_verbose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/address_verbose/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11886 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12753 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/date_to_block/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/date_to_block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10199 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/date_to_block/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_allowance/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_allowance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12641 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_allowance/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_price/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_price/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_transfers/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata_symbols/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata_symbols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata_symbols/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/info_endpoint_weights/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/info_endpoint_weights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/info_endpoint_weights/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.875042 moralis-0.1.9/src/openapi_evm_api/paths/ipfs_upload_folder/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/ipfs_upload_folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13228 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/ipfs_upload_folder/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14247 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_lowestprice/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_lowestprice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_lowestprice/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12028 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_metadata/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_owners/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_owners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13484 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_owners/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_sync/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13112 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_owners/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_owners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_owners/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_transfers/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_trades/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_trades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_trades/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_address_transfers/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_get_multiple_nfts/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_get_multiple_nfts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14571 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_get_multiple_nfts/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_search/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/nft_transfers/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/nft_transfers/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/pair_address_reserves/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/pair_address_reserves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14700 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/pair_address_reserves/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/resolve_address_reverse/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/resolve_address_reverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/resolve_address_reverse/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/resolve_domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/resolve_domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/resolve_domain/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.879042 moralis-0.1.9/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.883042 moralis-0.1.9/src/openapi_evm_api/paths/transaction_transaction_hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/transaction_transaction_hash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11970 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/transaction_transaction_hash/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.883042 moralis-0.1.9/src/openapi_evm_api/paths/web3_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/web3_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/paths/web3_version/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97681 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.883042 moralis-0.1.9/src/openapi_evm_api/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.887042 moralis-0.1.9/src/openapi_evm_api/test/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_block_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_block_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_chain_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_endpoint_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_ens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_allowance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_token_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc721_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_get_multiple_nfts_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_historical_nft_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_ipfs_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_ipfs_file_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log_event_by_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_metadata_resync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_native_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_native_erc20_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_contract_metadata_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_metadata_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_owner_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_transfer_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_wallet_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_normalized_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_normalized_metadata_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_reserves_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_reserves_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_run_contract_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_token_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_trade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_trade_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_transaction_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_transaction_collection_verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_evm_api/test/test_models/test_web3version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.887042 moralis-0.1.9/src/openapi_sol_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58533 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.887042 moralis-0.1.9/src/openapi_sol_api/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/path_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/apis/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/paths/account_network_address_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/paths/account_network_address_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/paths/account_network_address_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/paths/account_network_address_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/paths/nft_network_address_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/paths/token_network_address_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/tag_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/apis/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/tags/account_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/tags/nft_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/apis/tags/token_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/metaplex_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/native_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/nft_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/spl_native_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/spl_token_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/spl_token_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/model/splnft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_balance/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_balance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_balance/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_nft/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_nft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_nft/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_portfolio/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_portfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_portfolio/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_tokens/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_tokens/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/paths/nft_network_address_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/nft_network_address_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10852 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/nft_network_address_metadata/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/paths/token_network_address_price/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/token_network_address_price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/paths/token_network_address_price/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97596 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.891042 moralis-0.1.9/src/openapi_sol_api/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.895042 moralis-0.1.9/src/openapi_sol_api/test/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_metaplex_nft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_native_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_nft_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_spl_native_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_spl_token_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_spl_token_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_sol_api/test/test_models/test_splnft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.895042 moralis-0.1.9/src/openapi_streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58561 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.895042 moralis-0.1.9/src/openapi_streams/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/path_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.895042 moralis-0.1.9/src/openapi_streams/apis/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/history_replay_stream_id_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/stats_stream_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/streams_evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/streams_evm_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/streams_evm_id_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/paths/streams_evm_id_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/tag_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.895042 moralis-0.1.9/src/openapi_streams/apis/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/tags/evm_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/tags/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/tags/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/apis/tags/stats_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4486 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/abi_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/abi_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/abi_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5637 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/addresses_types_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/addresses_types_addresses_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/addresses_types_addresses_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/addresses_types_addresses_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/addresses_types_delete_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/addresses_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/advanced_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/history_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/history_types_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/history_types_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/history_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/internal_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/partial_streams_types_streams_model_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/settings_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/settings_types_settings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/stream_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13594 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_types_streams_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_types_streams_model_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_types_streams_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_types_streams_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/streams_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21422 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/usagestats_types_usage_stats_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4445 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/webhook_types_i_tiny_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/model/webhook_types_i_webhook_un_parsed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10520 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/history/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/history_replay_stream_id_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/history_replay_stream_id_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/history_replay_stream_id_id/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/settings/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/settings/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/stats/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/stats_stream_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/stats_stream_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9919 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/stats_stream_id/get.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/streams_evm/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm/put.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13891 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14073 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_status/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_status/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97624 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.903042 moralis-0.1.9/src/openapi_streams/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:54.907042 moralis-0.1.9/src/openapi_streams/test/test_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_abi_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_abi_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_abi_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_addresses_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_addresses_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_addresses_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_delete_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_advanced_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_history_types_history_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_history_types_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_history_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_internal_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_partial_streams_types_streams_model_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_settings_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_settings_types_settings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_stream_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_model_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_status_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_usagestats_types_usage_stats_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_webhook_types_i_tiny_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2022-12-13 20:15:40.000000 moralis-0.1.9/src/openapi_streams/test/test_models/test_webhook_types_i_webhook_un_parsed.py
```

### Comparing `moralis-0.1.8/LICENCE.md` & `moralis-0.1.9/LICENCE.md`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/PKG-INFO` & `moralis-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moralis
-Version: 0.1.8
+Version: 0.1.9
 Summary: The official Moralis Python SDK
 Keywords: Moralis,Moralis SDK,Moralis Python SDK,Web3,Crypto,Ethereum,Avalanche,Blockchain,Contracts,Eth,Evm,Fantom,Nft,Dapps,Binance,Solana
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moralis Version: 0.1.8 Summary: The official
+Metadata-Version: 2.1 Name: moralis Version: 0.1.9 Summary: The official
 Moralis Python SDK Keywords: Moralis,Moralis SDK,Moralis Python
 SDK,Web3,Crypto,Ethereum,Avalanche,Blockchain,Contracts,Eth,Evm,Fantom,Nft,Dapps,Binance,Solana
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE.md
                                [Moralis_JS_SDK]
                        ****** Moralis Python SDK ******
      [Join_the_Moralis_DAO_on_Discord] [Check_the_docs] [Discourse_posts]
```

### Comparing `moralis-0.1.8/README.md` & `moralis-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/setup.py` & `moralis-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "python-dateutil ~= 2.7.0",
     "typing_extensions ~= 4.3.0",
     "urllib3 ~= 1.26.7",
 ]
 
 setup(
     name="moralis",
-    version="0.1.8",
+    version="0.1.9",
     description="The official Moralis Python SDK",
     keywords=["Moralis", "Moralis SDK", "Moralis Python SDK", "Web3", "Crypto", "Ethereum", "Avalanche",
               "Blockchain", "Contracts", "Eth", "Evm", "Fantom", "Nft", "Dapps", "Binance", "Solana"],
     python_requires=">=3.7",
     install_requires=REQUIRES,
     package_dir={'': 'src'},
     packages=find_packages('src'),
```

### Comparing `moralis-0.1.8/src/moralis/auth/challenge/api_instance.py` & `moralis-0.1.9/src/moralis/auth/challenge/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/auth/challenge/request_challenge_solana.py` & `moralis-0.1.9/src/moralis/auth/challenge/request_challenge_solana.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/auth/challenge/verify_challenge_solana.py` & `moralis-0.1.9/src/moralis/auth/challenge/verify_challenge_solana.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/balance/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/balance/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/balance/get_native_balance.py` & `moralis-0.1.9/src/moralis/evm_api/balance/get_native_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/block/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/block/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/block/get_block.py` & `moralis-0.1.9/src/moralis/evm_api/block/get_block.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/block/get_date_to_block.py` & `moralis-0.1.9/src/moralis/evm_api/block/get_date_to_block.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/defi/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/defi/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/defi/get_pair_address.py` & `moralis-0.1.9/src/moralis/evm_api/defi/get_pair_address.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/defi/get_pair_reserves.py` & `moralis-0.1.9/src/moralis/evm_api/defi/get_pair_reserves.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/events/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/events/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/events/get_contract_events.py` & `moralis-0.1.9/src/moralis/evm_api/events/get_contract_events.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/events/get_contract_logs.py` & `moralis-0.1.9/src/moralis/evm_api/events/get_contract_logs.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/ipfs/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/ipfs/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/nft/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_contract_nfts.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_contract_nfts.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_multiple_nfts.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_multiple_nfts.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_contract_metadata.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_contract_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_contract_transfers.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_contract_transfers.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_lowest_price.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_lowest_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_metadata.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_owners.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_owners.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_token_id_owners.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_token_id_owners.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_trades.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_trades.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_transfers.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_transfers.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_transfers_by_block.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_transfers_by_block.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_nft_transfers_from_to_block.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_nft_transfers_from_to_block.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_wallet_nft_collections.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_wallet_nft_collections.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_wallet_nft_transfers.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_wallet_nft_transfers.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/get_wallet_nfts.py` & `moralis-0.1.9/src/moralis/evm_api/nft/get_wallet_nfts.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/nft.py` & `moralis-0.1.9/src/moralis/evm_api/nft/nft.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/re_sync_metadata.py` & `moralis-0.1.9/src/moralis/evm_api/nft/re_sync_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/search_nfts.py` & `moralis-0.1.9/src/moralis/evm_api/nft/search_nfts.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/nft/sync_nft_contract.py` & `moralis-0.1.9/src/moralis/evm_api/nft/sync_nft_contract.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/resolve/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/resolve/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/resolve/resolve_address.py` & `moralis-0.1.9/src/moralis/evm_api/resolve/resolve_address.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/resolve/resolve_domain.py` & `moralis-0.1.9/src/moralis/evm_api/resolve/resolve_domain.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/token/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/get_token_allowance.py` & `moralis-0.1.9/src/moralis/evm_api/token/get_token_allowance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/get_token_metadata.py` & `moralis-0.1.9/src/moralis/evm_api/token/get_token_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/get_token_metadata_by_symbol.py` & `moralis-0.1.9/src/moralis/evm_api/token/get_token_metadata_by_symbol.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/get_token_price.py` & `moralis-0.1.9/src/moralis/evm_api/token/get_token_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/get_token_transfers.py` & `moralis-0.1.9/src/moralis/evm_api/token/get_token_transfers.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/get_wallet_token_balances.py` & `moralis-0.1.9/src/moralis/evm_api/token/get_wallet_token_balances.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/token/get_wallet_token_transfers.py` & `moralis-0.1.9/src/moralis/evm_api/token/get_wallet_token_transfers.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/transaction/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/transaction/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/transaction/get_transaction.py` & `moralis-0.1.9/src/moralis/evm_api/transaction/get_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/transaction/get_wallet_transactions.py` & `moralis-0.1.9/src/moralis/evm_api/transaction/get_wallet_transactions.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/transaction/get_wallet_transactions_verbose.py` & `moralis-0.1.9/src/moralis/evm_api/transaction/get_wallet_transactions_verbose.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/utils/api_instance.py` & `moralis-0.1.9/src/moralis/evm_api/utils/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/evm_api/utils/run_contract_function.py` & `moralis-0.1.9/src/moralis/evm_api/utils/run_contract_function.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/account/api_instance.py` & `moralis-0.1.9/src/moralis/sol_api/account/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/account/balance.py` & `moralis-0.1.9/src/moralis/sol_api/account/balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/account/get_nfts.py` & `moralis-0.1.9/src/moralis/sol_api/account/get_nfts.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/account/get_portfolio.py` & `moralis-0.1.9/src/moralis/sol_api/account/get_portfolio.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/account/get_spl.py` & `moralis-0.1.9/src/moralis/sol_api/account/get_spl.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/nft/api_instance.py` & `moralis-0.1.9/src/moralis/sol_api/nft/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/nft/get_nft_metadata.py` & `moralis-0.1.9/src/moralis/sol_api/nft/get_nft_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/token/api_instance.py` & `moralis-0.1.9/src/moralis/sol_api/token/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/sol_api/token/get_token_price.py` & `moralis-0.1.9/src/moralis/sol_api/token/get_token_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/add_address_to_stream.py` & `moralis-0.1.9/src/moralis/streams/evm/add_address_to_stream.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/api_instance.py` & `moralis-0.1.9/src/moralis/streams/evm/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/delete_address_from_stream.py` & `moralis-0.1.9/src/moralis/streams/evm/delete_address_from_stream.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/delete_stream.py` & `moralis-0.1.9/src/moralis/streams/evm/delete_stream.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/get_addresses.py` & `moralis-0.1.9/src/moralis/streams/evm/get_addresses.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/get_stream.py` & `moralis-0.1.9/src/moralis/streams/evm/get_stream.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/get_streams.py` & `moralis-0.1.9/src/moralis/streams/evm/get_streams.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/update_stream.py` & `moralis-0.1.9/src/moralis/streams/evm/update_stream.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/evm/update_stream_status.py` & `moralis-0.1.9/src/moralis/streams/evm/update_stream_status.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/history/api_instance.py` & `moralis-0.1.9/src/moralis/streams/history/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/history/get_history.py` & `moralis-0.1.9/src/moralis/streams/history/get_history.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/history/replay_history.py` & `moralis-0.1.9/src/moralis/streams/history/replay_history.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/project/api_instance.py` & `moralis-0.1.9/src/moralis/streams/project/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/stats/api_instance.py` & `moralis-0.1.9/src/moralis/streams/stats/api_instance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis/streams/stats/get_stats_by_stream_id.py` & `moralis-0.1.9/src/moralis/streams/stats/get_stats_by_stream_id.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/moralis.egg-info/PKG-INFO` & `moralis-0.1.9/src/moralis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moralis
-Version: 0.1.8
+Version: 0.1.9
 Summary: The official Moralis Python SDK
 Keywords: Moralis,Moralis SDK,Moralis Python SDK,Web3,Crypto,Ethereum,Avalanche,Blockchain,Contracts,Eth,Evm,Fantom,Nft,Dapps,Binance,Solana
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moralis Version: 0.1.8 Summary: The official
+Metadata-Version: 2.1 Name: moralis Version: 0.1.9 Summary: The official
 Moralis Python SDK Keywords: Moralis,Moralis SDK,Moralis Python
 SDK,Web3,Crypto,Ethereum,Avalanche,Blockchain,Contracts,Eth,Evm,Fantom,Nft,Dapps,Binance,Solana
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE.md
                                [Moralis_JS_SDK]
                        ****** Moralis Python SDK ******
      [Join_the_Moralis_DAO_on_Discord] [Check_the_docs] [Discourse_posts]
```

### Comparing `moralis-0.1.8/src/moralis.egg-info/SOURCES.txt` & `moralis-0.1.9/src/moralis.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 src/moralis.egg-info/SOURCES.txt
 src/moralis.egg-info/dependency_links.txt
 src/moralis.egg-info/requires.txt
 src/moralis.egg-info/top_level.txt
 src/moralis/auth/__init__.py
 src/moralis/auth/auth.py
 src/moralis/auth/utilities.py
+src/moralis/auth/version.py
 src/moralis/auth/challenge/__init__.py
 src/moralis/auth/challenge/api_instance.py
 src/moralis/auth/challenge/challenge.py
 src/moralis/auth/challenge/request_challenge_evm.py
 src/moralis/auth/challenge/request_challenge_solana.py
 src/moralis/auth/challenge/verify_challenge_evm.py
 src/moralis/auth/challenge/verify_challenge_solana.py
 src/moralis/evm_api/__init__.py
 src/moralis/evm_api/evm_api.py
 src/moralis/evm_api/utilities.py
+src/moralis/evm_api/version.py
 src/moralis/evm_api/balance/__init__.py
 src/moralis/evm_api/balance/api_instance.py
 src/moralis/evm_api/balance/balance.py
 src/moralis/evm_api/balance/get_native_balance.py
 src/moralis/evm_api/block/__init__.py
 src/moralis/evm_api/block/api_instance.py
 src/moralis/evm_api/block/block.py
@@ -90,14 +92,15 @@
 src/moralis/evm_api/utils/endpoint_weights.py
 src/moralis/evm_api/utils/run_contract_function.py
 src/moralis/evm_api/utils/utils.py
 src/moralis/evm_api/utils/web3_api_version.py
 src/moralis/sol_api/__init__.py
 src/moralis/sol_api/sol_api.py
 src/moralis/sol_api/utilities.py
+src/moralis/sol_api/version.py
 src/moralis/sol_api/account/__init__.py
 src/moralis/sol_api/account/account.py
 src/moralis/sol_api/account/api_instance.py
 src/moralis/sol_api/account/balance.py
 src/moralis/sol_api/account/get_nfts.py
 src/moralis/sol_api/account/get_portfolio.py
 src/moralis/sol_api/account/get_spl.py
@@ -108,14 +111,15 @@
 src/moralis/sol_api/token/__init__.py
 src/moralis/sol_api/token/api_instance.py
 src/moralis/sol_api/token/get_token_price.py
 src/moralis/sol_api/token/token.py
 src/moralis/streams/__init__.py
 src/moralis/streams/streams.py
 src/moralis/streams/utilities.py
+src/moralis/streams/version.py
 src/moralis/streams/evm/__init__.py
 src/moralis/streams/evm/add_address_to_stream.py
 src/moralis/streams/evm/api_instance.py
 src/moralis/streams/evm/create_stream.py
 src/moralis/streams/evm/delete_address_from_stream.py
 src/moralis/streams/evm/delete_stream.py
 src/moralis/streams/evm/evm.py
```

### Comparing `moralis-0.1.8/src/openapi_auth/__init__.py` & `moralis-0.1.9/src/openapi_auth/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/api_client.py` & `moralis-0.1.9/src/openapi_auth/api_client.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/apis/path_to_api.py` & `moralis-0.1.9/src/openapi_auth/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/apis/tags/challenge_api.py` & `moralis-0.1.9/src/openapi_auth/apis/tags/challenge_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/configuration.py` & `moralis-0.1.9/src/openapi_auth/configuration.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/exceptions.py` & `moralis-0.1.9/src/openapi_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/evm_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/model/evm_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/evm_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/model/evm_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/evm_complete_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/model/evm_complete_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/evm_complete_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/model/evm_complete_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/solana_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/model/solana_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/solana_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/model/solana_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/solana_complete_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/model/solana_complete_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/model/solana_complete_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/model/solana_complete_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/models/__init__.py` & `moralis-0.1.9/src/openapi_auth/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/paths/challenge_request_evm/post.py` & `moralis-0.1.9/src/openapi_auth/paths/challenge_request_evm/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/paths/challenge_request_solana/post.py` & `moralis-0.1.9/src/openapi_auth/paths/challenge_request_solana/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/paths/challenge_verify_evm/post.py` & `moralis-0.1.9/src/openapi_auth/paths/challenge_verify_evm/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/paths/challenge_verify_solana/post.py` & `moralis-0.1.9/src/openapi_auth/paths/challenge_verify_solana/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/rest.py` & `moralis-0.1.9/src/openapi_auth/rest.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/schemas.py` & `moralis-0.1.9/src/openapi_auth/schemas.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_complete_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_complete_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_evm_complete_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_evm_complete_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_complete_challenge_request_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_complete_challenge_request_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_auth/test/test_models/test_solana_complete_challenge_response_dto.py` & `moralis-0.1.9/src/openapi_auth/test/test_models/test_solana_complete_challenge_response_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/__init__.py` & `moralis-0.1.9/src/openapi_evm_api/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/api_client.py` & `moralis-0.1.9/src/openapi_evm_api/api_client.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/path_to_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tag_to_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/balance_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/balance_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/block_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/block_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/defi_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/defi_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/events_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/events_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/ipfs_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/ipfs_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/nft_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/nft_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/resolve_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/resolve_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/token_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/token_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/transaction_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/transaction_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/apis/tags/utils_api.py` & `moralis-0.1.9/src/openapi_evm_api/apis/tags/utils_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/configuration.py` & `moralis-0.1.9/src/openapi_evm_api/configuration.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/exceptions.py` & `moralis-0.1.9/src/openapi_evm_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/block.py` & `moralis-0.1.9/src/openapi_evm_api/model/block.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/block_date.py` & `moralis-0.1.9/src/openapi_evm_api/model/block_date.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/block_transaction.py` & `moralis-0.1.9/src/openapi_evm_api/model/block_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/chain_list.py` & `moralis-0.1.9/src/openapi_evm_api/model/chain_list.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/endpoint_weights.py` & `moralis-0.1.9/src/openapi_evm_api/model/endpoint_weights.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/ens.py` & `moralis-0.1.9/src/openapi_evm_api/model/ens.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/erc20_allowance.py` & `moralis-0.1.9/src/openapi_evm_api/model/erc20_allowance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/erc20_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/model/erc20_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/erc20_price.py` & `moralis-0.1.9/src/openapi_evm_api/model/erc20_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/erc20_token_balance.py` & `moralis-0.1.9/src/openapi_evm_api/model/erc20_token_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/erc20_transaction.py` & `moralis-0.1.9/src/openapi_evm_api/model/erc20_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/erc20_transaction_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/erc20_transaction_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/erc721_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/model/erc721_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/get_multiple_nfts_dto.py` & `moralis-0.1.9/src/openapi_evm_api/model/get_multiple_nfts_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/historical_nft_transfer.py` & `moralis-0.1.9/src/openapi_evm_api/model/historical_nft_transfer.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/ipfs_file.py` & `moralis-0.1.9/src/openapi_evm_api/model/ipfs_file.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/ipfs_file_request.py` & `moralis-0.1.9/src/openapi_evm_api/model/ipfs_file_request.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/log.py` & `moralis-0.1.9/src/openapi_evm_api/model/log.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/log_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/log_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/log_event.py` & `moralis-0.1.9/src/openapi_evm_api/model/log_event.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/log_event_by_address.py` & `moralis-0.1.9/src/openapi_evm_api/model/log_event_by_address.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/metadata_resync.py` & `moralis-0.1.9/src/openapi_evm_api/model/metadata_resync.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/native_balance.py` & `moralis-0.1.9/src/openapi_evm_api/model/native_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/native_erc20_price.py` & `moralis-0.1.9/src/openapi_evm_api/model/native_erc20_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_collections.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_collections.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_contract_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_contract_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_contract_metadata_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_contract_metadata_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_metadata_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_metadata_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_owner.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_owner.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_owner_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_owner_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_transfer.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_transfer.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_transfer_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_transfer_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/nft_wallet_collections.py` & `moralis-0.1.9/src/openapi_evm_api/model/nft_wallet_collections.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/normalized_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/model/normalized_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/normalized_metadata_attribute.py` & `moralis-0.1.9/src/openapi_evm_api/model/normalized_metadata_attribute.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/reserves_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/reserves_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/reserves_pair.py` & `moralis-0.1.9/src/openapi_evm_api/model/reserves_pair.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/resolve.py` & `moralis-0.1.9/src/openapi_evm_api/model/resolve.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/run_contract_dto.py` & `moralis-0.1.9/src/openapi_evm_api/model/run_contract_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/token_item.py` & `moralis-0.1.9/src/openapi_evm_api/model/token_item.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/trade.py` & `moralis-0.1.9/src/openapi_evm_api/model/trade.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/trade_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/trade_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/transaction.py` & `moralis-0.1.9/src/openapi_evm_api/model/transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/transaction_collection.py` & `moralis-0.1.9/src/openapi_evm_api/model/transaction_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/transaction_collection_verbose.py` & `moralis-0.1.9/src/openapi_evm_api/model/transaction_collection_verbose.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/model/web3version.py` & `moralis-0.1.9/src/openapi_evm_api/model/web3version.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/models/__init__.py` & `moralis-0.1.9/src/openapi_evm_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/__init__.py` & `moralis-0.1.9/src/openapi_evm_api/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_balance/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_balance/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_erc20/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_erc20/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_erc20_transfers/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_erc20_transfers/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_events/post.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_events/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_function/post.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_function/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_logs/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_logs/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_nft/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_nft/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_nft_collections/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_nft_collections/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_nft_transfers/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_nft_transfers/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/address_verbose/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/address_verbose/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/block_block_number_or_hash_nft_transfers/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/date_to_block/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/date_to_block/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_allowance/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_allowance/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_price/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_price/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/erc20_address_transfers/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/erc20_address_transfers/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/erc20_metadata_symbols/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/erc20_metadata_symbols/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/info_endpoint_weights/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/info_endpoint_weights/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/ipfs_upload_folder/post.py` & `moralis-0.1.9/src/openapi_evm_api/paths/ipfs_upload_folder/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_lowestprice/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_lowestprice/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_metadata/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_metadata/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_owners/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_owners/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_sync/put.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_sync/put.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_metadata_resync/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_owners/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_owners/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_token_id_transfers/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_token_id_transfers/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_trades/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_trades/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_address_transfers/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_address_transfers/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_get_multiple_nfts/post.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_get_multiple_nfts/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_search/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_search/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/nft_transfers/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/nft_transfers/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/pair_address_reserves/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/pair_address_reserves/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/resolve_address_reverse/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/resolve_address_reverse/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/resolve_domain/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/resolve_domain/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/token0_address_token1_address_pair_address/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/transaction_transaction_hash/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/transaction_transaction_hash/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/paths/web3_version/get.py` & `moralis-0.1.9/src/openapi_evm_api/paths/web3_version/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/rest.py` & `moralis-0.1.9/src/openapi_evm_api/rest.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/schemas.py` & `moralis-0.1.9/src/openapi_evm_api/schemas.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_block.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_block.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_block_date.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_block_date.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_block_transaction.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_block_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_chain_list.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_chain_list.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_endpoint_weights.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_endpoint_weights.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_ens.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_ens.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_allowance.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_allowance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_price.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_token_balance.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_token_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_transaction.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc20_transaction_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc20_transaction_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_erc721_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_erc721_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_get_multiple_nfts_dto.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_get_multiple_nfts_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_historical_nft_transfer.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_historical_nft_transfer.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_ipfs_file.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_ipfs_file.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_ipfs_file_request.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_ipfs_file_request.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log_event.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log_event.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_log_event_by_address.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_log_event_by_address.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_metadata_resync.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_metadata_resync.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_native_balance.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_native_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_native_erc20_price.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_native_erc20_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_collections.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_collections.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_contract_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_contract_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_contract_metadata_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_contract_metadata_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_metadata_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_metadata_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_owner.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_owner.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_owner_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_owner_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_transfer.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_transfer.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_transfer_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_transfer_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_nft_wallet_collections.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_nft_wallet_collections.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_normalized_metadata.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_normalized_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_normalized_metadata_attribute.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_normalized_metadata_attribute.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_reserves_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_reserves_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_reserves_pair.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_reserves_pair.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_resolve.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_resolve.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_run_contract_dto.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_run_contract_dto.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_token_item.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_token_item.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_trade.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_trade.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_trade_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_trade_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_transaction.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_transaction_collection.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_transaction_collection.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_transaction_collection_verbose.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_transaction_collection_verbose.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_evm_api/test/test_models/test_web3version.py` & `moralis-0.1.9/src/openapi_evm_api/test/test_models/test_web3version.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/__init__.py` & `moralis-0.1.9/src/openapi_sol_api/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/api_client.py` & `moralis-0.1.9/src/openapi_sol_api/api_client.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/apis/path_to_api.py` & `moralis-0.1.9/src/openapi_sol_api/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/apis/tag_to_api.py` & `moralis-0.1.9/src/openapi_sol_api/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/apis/tags/account_api.py` & `moralis-0.1.9/src/openapi_sol_api/apis/tags/account_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/configuration.py` & `moralis-0.1.9/src/openapi_sol_api/configuration.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/exceptions.py` & `moralis-0.1.9/src/openapi_sol_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/metaplex_nft.py` & `moralis-0.1.9/src/openapi_sol_api/model/metaplex_nft.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/native_balance.py` & `moralis-0.1.9/src/openapi_sol_api/model/native_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/nft_metadata.py` & `moralis-0.1.9/src/openapi_sol_api/model/nft_metadata.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/portfolio.py` & `moralis-0.1.9/src/openapi_sol_api/model/portfolio.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/spl_native_price.py` & `moralis-0.1.9/src/openapi_sol_api/model/spl_native_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/spl_token_balance.py` & `moralis-0.1.9/src/openapi_sol_api/model/spl_token_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/spl_token_price.py` & `moralis-0.1.9/src/openapi_sol_api/model/spl_token_price.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/model/splnft.py` & `moralis-0.1.9/src/openapi_sol_api/model/splnft.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/models/__init__.py` & `moralis-0.1.9/src/openapi_sol_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/paths/__init__.py` & `moralis-0.1.9/src/openapi_sol_api/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_balance/get.py` & `moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_balance/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_nft/get.py` & `moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_nft/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_portfolio/get.py` & `moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_portfolio/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/paths/account_network_address_tokens/get.py` & `moralis-0.1.9/src/openapi_sol_api/paths/account_network_address_tokens/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/paths/nft_network_address_metadata/get.py` & `moralis-0.1.9/src/openapi_sol_api/paths/nft_network_address_metadata/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/paths/token_network_address_price/get.py` & `moralis-0.1.9/src/openapi_sol_api/paths/token_network_address_price/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/rest.py` & `moralis-0.1.9/src/openapi_sol_api/rest.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/schemas.py` & `moralis-0.1.9/src/openapi_sol_api/schemas.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_sol_api/test/test_models/test_spl_token_balance.py` & `moralis-0.1.9/src/openapi_sol_api/test/test_models/test_spl_token_balance.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/__init__.py` & `moralis-0.1.9/src/openapi_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/api_client.py` & `moralis-0.1.9/src/openapi_streams/api_client.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/apis/path_to_api.py` & `moralis-0.1.9/src/openapi_streams/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/apis/tag_to_api.py` & `moralis-0.1.9/src/openapi_streams/apis/tag_to_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/apis/tags/evm_api.py` & `moralis-0.1.9/src/openapi_streams/apis/tags/evm_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/apis/tags/history_api.py` & `moralis-0.1.9/src/openapi_streams/apis/tags/history_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/apis/tags/project_api.py` & `moralis-0.1.9/src/openapi_streams/apis/tags/project_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/apis/tags/stats_api.py` & `moralis-0.1.9/src/openapi_streams/apis/tags/stats_api.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/configuration.py` & `moralis-0.1.9/src/openapi_streams/configuration.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/exceptions.py` & `moralis-0.1.9/src/openapi_streams/exceptions.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/abi_input.py` & `moralis-0.1.9/src/openapi_streams/model/abi_input.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/abi_item.py` & `moralis-0.1.9/src/openapi_streams/model/abi_item.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/abi_output.py` & `moralis-0.1.9/src/openapi_streams/model/abi_output.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/addresses.py` & `moralis-0.1.9/src/openapi_streams/model/addresses.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/addresses_types_address_response.py` & `moralis-0.1.9/src/openapi_streams/model/addresses_types_address_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/addresses_types_addresses_add.py` & `moralis-0.1.9/src/openapi_streams/model/addresses_types_addresses_add.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/addresses_types_addresses_remove.py` & `moralis-0.1.9/src/openapi_streams/model/addresses_types_addresses_remove.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/addresses_types_addresses_response.py` & `moralis-0.1.9/src/openapi_streams/model/addresses_types_addresses_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/addresses_types_delete_address_response.py` & `moralis-0.1.9/src/openapi_streams/model/addresses_types_delete_address_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/addresses_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/model/addresses_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/advanced_options.py` & `moralis-0.1.9/src/openapi_streams/model/advanced_options.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/block.py` & `moralis-0.1.9/src/openapi_streams/model/block.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/history_model.py` & `moralis-0.1.9/src/openapi_streams/model/history_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/history_types_history_model.py` & `moralis-0.1.9/src/openapi_streams/model/history_types_history_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/history_types_history_response.py` & `moralis-0.1.9/src/openapi_streams/model/history_types_history_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/history_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/model/history_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/internal_transaction.py` & `moralis-0.1.9/src/openapi_streams/model/internal_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/log.py` & `moralis-0.1.9/src/openapi_streams/model/log.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/partial_streams_types_streams_model_create.py` & `moralis-0.1.9/src/openapi_streams/model/partial_streams_types_streams_model_create.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/settings_region.py` & `moralis-0.1.9/src/openapi_streams/model/settings_region.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/settings_types_settings_model.py` & `moralis-0.1.9/src/openapi_streams/model/settings_types_settings_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/stream_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/model/stream_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_filter.py` & `moralis-0.1.9/src/openapi_streams/model/streams_filter.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_model.py` & `moralis-0.1.9/src/openapi_streams/model/streams_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_status.py` & `moralis-0.1.9/src/openapi_streams/model/streams_status.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_types_streams_model.py` & `moralis-0.1.9/src/openapi_streams/model/streams_types_streams_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_types_streams_model_create.py` & `moralis-0.1.9/src/openapi_streams/model/streams_types_streams_model_create.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_types_streams_response.py` & `moralis-0.1.9/src/openapi_streams/model/streams_types_streams_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_types_streams_status_update.py` & `moralis-0.1.9/src/openapi_streams/model/streams_types_streams_status_update.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/streams_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/model/streams_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/transaction.py` & `moralis-0.1.9/src/openapi_streams/model/transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/usagestats_types_usage_stats_model.py` & `moralis-0.1.9/src/openapi_streams/model/usagestats_types_usage_stats_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/uuid.py` & `moralis-0.1.9/src/openapi_streams/model/uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/webhook_types_i_tiny_payload.py` & `moralis-0.1.9/src/openapi_streams/model/webhook_types_i_tiny_payload.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/model/webhook_types_i_webhook_un_parsed.py` & `moralis-0.1.9/src/openapi_streams/model/webhook_types_i_webhook_un_parsed.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/models/__init__.py` & `moralis-0.1.9/src/openapi_streams/models/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/__init__.py` & `moralis-0.1.9/src/openapi_streams/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/history/get.py` & `moralis-0.1.9/src/openapi_streams/paths/history/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/history_replay_stream_id_id/post.py` & `moralis-0.1.9/src/openapi_streams/paths/history_replay_stream_id_id/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/settings/get.py` & `moralis-0.1.9/src/openapi_streams/paths/settings/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/settings/post.py` & `moralis-0.1.9/src/openapi_streams/paths/settings/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/stats/get.py` & `moralis-0.1.9/src/openapi_streams/paths/stats/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/stats_stream_id/get.py` & `moralis-0.1.9/src/openapi_streams/paths/stats_stream_id/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm/get.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm/put.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm/put.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/delete.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/delete.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/get.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm_id/post.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm_id/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/delete.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/delete.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/get.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/get.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_address/post.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_address/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/paths/streams_evm_id_status/post.py` & `moralis-0.1.9/src/openapi_streams/paths/streams_evm_id_status/post.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/rest.py` & `moralis-0.1.9/src/openapi_streams/rest.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/schemas.py` & `moralis-0.1.9/src/openapi_streams/schemas.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_abi_input.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_abi_input.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_abi_output.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_abi_output.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_address_response.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_address_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_addresses_add.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_addresses_add.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_addresses_remove.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_addresses_remove.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_addresses_response.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_addresses_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_delete_address_response.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_delete_address_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_addresses_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_addresses_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_advanced_options.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_advanced_options.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_history_model.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_history_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_history_types_history_model.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_history_types_history_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_history_types_history_response.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_history_types_history_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_history_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_history_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_internal_transaction.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_internal_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_partial_streams_types_streams_model_create.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_partial_streams_types_streams_model_create.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_settings_region.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_settings_region.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_settings_types_settings_model.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_settings_types_settings_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_stream_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_stream_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_filter.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_filter.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_model.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_status.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_status.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_model.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_model_create.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_model_create.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_response.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_response.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_streams_status_update.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_streams_status_update.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_streams_types_uuid.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_streams_types_uuid.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_transaction.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_transaction.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_usagestats_types_usage_stats_model.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_usagestats_types_usage_stats_model.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_webhook_types_i_tiny_payload.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_webhook_types_i_tiny_payload.py`

 * *Files identical despite different names*

### Comparing `moralis-0.1.8/src/openapi_streams/test/test_models/test_webhook_types_i_webhook_un_parsed.py` & `moralis-0.1.9/src/openapi_streams/test/test_models/test_webhook_types_i_webhook_un_parsed.py`

 * *Files identical despite different names*

