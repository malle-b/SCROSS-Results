- FF lambda cut tuning on low statistics as a result of previous cuts. Should redo with more statistics.
- FF lambda vtx based cuts expected to be kind of bas since z resolution is poor. 
- MM cut tuning looks promising but should look at the distribution in data before I move this from 0. Looks like it can separate quite a lot of bg even in simulations, though. 
- PVA is an important cut and is probably best tuned with FoM. Sadly it seems broken. 
- All lambda: should I really remove dec_vtx_z? It does remove a lot of background, but sadly along with quite a lot of signal. Probably works best for HH and FH. *I need to examine a bigger negative range for dec_vtx_z*
- Something is very wrong with the PVA calculation, as is evident in HH lambda. 
- Determine what cuts removed signal in FF lambda data. *Answer*: There was very little signal to begin with. What is the reason for these low statistics? kIsUsedFlag? Should be better in gen4. 


ff_lambda_cuts_fracTuned_lambda_point_vec_min   -7
ff_lambda_cuts_fracTuned_prim_vtx_z_min   -259.2
ff_lambda_cuts_fracTuned_prim_vtx_z_max   54
*ff_lambda_cuts_fracTuned_track_dist_max   15.06 REMOVE, no good separation between bg and sig*
*ff_lambda_cuts_fracTuned_dec_vtx_z_min   -91 REMOVE, no good separation between bg and sig*
ff_lambda_cuts_fracTuned_PVA_max   0.5 *bad cut tuning, eyeballed instead*
ff_lambda_cuts_fracTuned_MM_min   0 *keep at 0. Remember hypsel does not read this from sproutparam*
*ff_lambda_cuts_fracTuned_vtx_dist_min   4 REMOVE, no good separation between bg and sig*
ff_sigma_cuts_fracTuned_missing_mass_min  1461.95  *stat too low for tuning. Used FH sigma cut instead*

fh_lambda_cuts_fracTuned_lambda_point_vec_min   -1.5
fh_lambda_cuts_fracTuned_prim_vtx_z_min   -172.8
fh_lambda_cuts_fracTuned_prim_vtx_z_max   -75.6
fh_lambda_cuts_fracTuned_track_dist_max   20.89 **IS THIS CUT USEFUL OR SHOULD I REMOVER?**
*fh_lambda_cuts_fracTuned_dec_vtx_z_min   -88 REMOVE, no good separation between bg and sig*
fh_lambda_cuts_fracTuned_PVA_max   0.75
fh_lambda_cuts_fracTuned_MM_min   0.3 *keep at 0. Remember hypsel does not read this from sproutparam*
*fh_lambda_cuts_fracTuned_vtx_dist_min   4 REMOVE; no good separation between bg and sig*
fh_sigma_cuts_fracTuned_missing_mass_min   1461.95

fw_track_cuts_fracTuned_tof_max   22
fw_track_cuts_fracTuned_chi2/ndf_max   3.4
fw_track_cuts_fracTuned_z_min   -247.6
fw_track_cuts_fracTuned_z_max   29.6

hf_lambda_cuts_fracTuned_lambda_point_vec_min   -1.5
hf_lambda_cuts_fracTuned_prim_vtx_z_min   -162
hf_lambda_cuts_fracTuned_prim_vtx_z_max   -75.6
*hf_lambda_cuts_fracTuned_track_dist_max   21.5 REMOVE, no good separation between bg and sig*
*hf_lambda_cuts_fracTuned_dec_vtx_z_min   -88 REMOVE; no good separation between bg and sig*
hf_lambda_cuts_fracTuned_PVA_max   0.75  *too generous. setting to fh lambda value*
hf_lambda_cuts_fracTuned_MM_min   0 *keep at 0. Remember hypsel does not read this from sproutparam*
*hf_lambda_cuts_fracTuned_vtx_dist_min   4 REMOVE; no ood separation between bg and sig*
hf_sigma_cuts_fracTuned_missing_mass_min   1491.95

hh_lambda_cuts_fracTuned_lambda_point_vec_min   -0.5
hh_lambda_cuts_fracTuned_prim_vtx_z_min   -162
hh_lambda_cuts_fracTuned_prim_vtx_z_max   129.6
hh_lambda_cuts_fracTuned_track_dist_max   18.56
hh_lambda_cuts_fracTuned_dec_vtx_z_min   -88
hh_lambda_cuts_fracTuned_PVA_max   1.59 *SOMETHING IS VERY WRONG*
hh_lambda_cuts_fracTuned_MM_min   0  *keep at 0. Remember hypsel does not read this from sproutparam*
*hh_lambda_cuts_fracTuned_vtx_dist_min   -0.5 REMOVE, no good separation between bg and sig*
hh_sigma_cuts_fracTuned_missing_mass_min   1371.95

prim_particle_cuts_fracTuned_z_min   -153.01
prim_particle_cuts_fracTuned_z_max   -93.99
