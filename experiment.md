# experiment

## build
* conda env: `conda activate urlb_test`

## walker domain
* pretrain: `python dreamer_pretrain.py configs=dmc_pixels agent=icm_dreamer domain=walker seed=1`
* finetune: `python dreamer_finetune_cuda4.py configs=dmc_pixels agent=icm_dreamer task=walker_flip snapshot_ts=500000 seed=1`
* finetune: `python dreamer_finetune_cuda5.py configs=dmc_pixels agent=icm_dreamer task=walker_run snapshot_ts=500000 seed=1`
* finetune: `python dreamer_finetune_cuda6.py configs=dmc_pixels agent=icm_dreamer task=walker_stand snapshot_ts=500000 seed=1`
* finetune: `python dreamer_finetune_cuda7.py configs=dmc_pixels agent=icm_dreamer task=walker_walk snapshot_ts=500000 seed=1`

## jaco domain
* pretrain: `python dreamer_pretrain_cuda1.py configs=dmc_pixels agent=icm_dreamer domain=jaco seed=1`
* finetune: `python dreamer_finetune_cuda4.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_top_left snapshot_ts=500000 seed=1`
* finetune: `python dreamer_finetune_cuda5.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_top_right snapshot_ts=500000 seed=1`
* finetune: `python dreamer_finetune_cuda6.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_bottom_left snapshot_ts=500000 seed=1`
* finetune: `python dreamer_finetune_cuda7.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_bottom_right snapshot_ts=500000 seed=1`

### alternative
* finetune: `python dreamer_finetune_cuda2.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_top_left snapshot_ts=100000 seed=1`
* finetune: `python dreamer_finetune_cuda2.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_top_right snapshot_ts=100000 seed=1`
* finetune: `python dreamer_finetune_cuda3.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_bottom_left snapshot_ts=100000 seed=1`
* finetune: `python dreamer_finetune_cuda3.py configs=dmc_pixels agent=icm_dreamer task=jaco_reach_bottom_right snapshot_ts=100000 seed=1`
