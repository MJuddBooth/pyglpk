Change LPX_solver_simplex, LPX_solver_integer to accept new control options.

Tests for...
LPX.erase()
Bar.scale

For each section of the GLPK 4.52 manual that describes functions,
this describes the progress in providing the functionality of that
procedure in PyGLPK, the corresponding C function, and the source file
in which the functionality is provided.  

# Chapter 2
## Section 2.3
* 2.3.1  Done, glp_create_prob (lp.c)
* 2.3.2  Done, glp_set_prob_name (lp.c)
* 2.3.3  Done, glp_set_obj_name (obj.c)
* 2.3.4  Done, glp_set_obj_dir (obj.c)
* 2.3.5  Done, glp_add_rows (barcol.c)
* 2.3.6  Done, glp_add_cols (barcol.c)
* 2.3.7  Done, glp_set_row_name (bar.c)
* 2.3.8  Done, glp_set_col_name (bar.c)
* 2.3.9  Done, glp_set_row_bnds (bar.c)
* 2.3.10 Done, glp_set_col_bnds (bar.c)
* 2.3.11 Done, glp_set_obj_coef (obj.c)
* 2.3.12 Done, glp_set_mat_row (bar.c)
* 2.3.13 Done, glp_set_mat_col (bar.c)
* 2.3.14 Done, glp_load_matrix (lp.c)
* 2.3.15 *Not done glp_check_dup
* 2.3.16 *Not done, glp_sort_matrix
* 2.3.17 Done, glp_del_rows (barcol.c)
* 2.3.18 Done, glp_del_cols (barcol.c)
* 2.3.19 *Not done, glp_copy_prob
* 2.3.20 Done, glp_erase_prob (lp.c)
* 2.3.21 Done, glp_delete_prob (lp.c)

## Section 2.4
* 2.4.1  Done, glp_get_prob_name (lp.c)
* 2.4.2  Done, glp_get_obj_name (obj.c)
* 2.4.3  Done, glp_get_obj_dir (obj.c)
* 2.4.4  Done, glp_get_num_rows (barcol.c)
* 2.4.5  Done, glp_get_num_cols (barcol.c)
* 2.4.6  Done, glp_get_row_name (bar.c)
* 2.4.7  Done, glp_get_col_name (bar.c)
* 2.4.8  Done, glp_get_row_type (bar.c)
* 2.4.9  Done, glp_get_row_lb (bar.c)
* 2.4.10 Done, glp_get_row_ub (bar.c)
* 2.4.11 Done, glp_get_col_type (bar.c)
* 2.4.12 Done, glp_get_col_lb (bar.c)
* 2.4.13 Done, glp_get_col_ub (bar.c)
* 2.4.14 Done, glp_get_obj_coef (obj.c)
* 2.4.15 Done, glp_get_num_nz (lp.c)
* 2.4.16 Done, glp_get_mat_row (bar.c)
* 2.4.17 Done, glp_get_mat_col (bar.c)

## Section 2.5  
* 2.5.1  Done, glp_create_index (barcol.c)
* 2.5.2  Done, glp_find_row (barcol.c)
* 2.5.3  Done, glp_find_col (barcol.c)
* 2.5.4  N/A, glp_delete_index (it is not exactly appropriate anywhere)

## Section 2.6  
* 2.6.2  Done, glp_set_rii (bar.c)
* 2.6.3  Done, glp_set_sjj (bar.c)
* 2.6.4  Done, glp_get_rii (bar.c)
* 2.6.5  Done, glp_get_sjj (bar.c)
* 2.6.6  Done, glp_scale_prob (lp.c)
* 2.6.7  Done, glp_unscale_prob (lp.c)
  
## Section 2.7
* 2.7.2  Done, glp_set_row_stat (bar.c)
* 2.7.3  Done, glp_set_col_stat (bar.c)
* 2.7.4  Done, glp_std_basis (lp.c)
* 2.7.5  Done, glp_adv_basis (lp.c)
* 2.7.6  Done, glp_cpx_basis (lp.c)

## Section 2.8
* 2.8.1  Done, glp_simplex (lp.c)
* 2.8.2  Done, lpx_exact (lp.c) - should this become glp_exact?
* 2.8.3  N/A, glp_init_smcp (we don't represent glp_smcp objects explicitly)
* 2.8.4  Done, glp_get_status (lp.c)
* 2.8.5  Done, glp_get_prim_stat (lp.c)
* 2.8.6  Done, glp_get_dual_stat (lp.c)
* 2.8.7  Done, glp_get_obj_val (obj.c)
* 2.8.8  Done, glp_get_row_stat (bar.c)
* 2.8.9  Done, glp_get_row_prim (bar.c)
* 2.8.10 Done, glp_get_row_dual (bar.c)
* 2.8.11 Done, glp_get_col_stat (bar.c)
* 2.8.12 Done, glp_get_col_prim (bar.c)
* 2.8.13 Done, glp_get_col_dual (bar.c)
* 2.8.14 Done, lpx_get_ray_info (lp.c)

## Section 2.9
* 2.9.1  Done, lpx_interior (lp.c)
* 2.9.2  ??
* 2.9.3  Done, glp_ipt_status (lp.c)
* 2.9.4  Done, glp_ipt_obj_val (lp.c)
* 2.9.5  Done, glp_int_row_prim (bar.c)
* 2.9.6  Done, glp_int_row_dual (bar.c)
* 2.9.7  Done, glp_int_col_prim (bar.c)
* 2.9.8  Done, glp_int_col_dual (bar.c)

## Section 2.10
* 2.10.1  Done, glp_set_col_kind (bar.c)
* 2.10.2  Done, glp_get_col_kind (bar.c)
* 2.10.3  Done, glp_get_num_int (lp.c)
* 2.10.4  Done, glp_get_num_bin (lp.c)
* 2.10.5  Done, glp_intopt (lp.c)
* 2.10.6  N/A, glp_init_iocp (we don't represent glp_iocp objects explicitly)
* 2.10.   Done, lpx_intopt (lp.c) - this is no longer supported by glpk
* 2.10.7  Done, glp_mip_status (lp.c)
* 2.10.8  Done, glp_mip_obj_val (obj.c)
* 2.10.9  Done, glp_mip_row_val (bar.c)
* 2.10.10 Done, glp_mip_col_val (bar.c)

# Section 2.11
* 2.11.1  Done, lpx_check_kkt (lp.c, kkt.c)

# Chapter 3
Changed a couple of the data reading and writing techniques, but frankly I don't care enough about reading problems from datafiles to stop relying upon the compatibility layer.

# Chapter 4
## Section 4.1
## Section 4.2
## Section 4.3
   All of this does not appear anywhere within PyGLPK.  The original author's feeling is
   that few will care about explicitly performing the steps of the
   simplex algorithm.
## Section 4.4 Post-optimal analysis routines
* 4.4.1 *To Do. glp_analyze_bound 
* 4.4.2 *To Do. glp_analyze_coef 

# Chapter 5
## Section 2
* 5.2.1  Done, glp_ios_reason (tree.c)
* 5.2.2  Done, glp_ios_get_prob (tree.c)
* 5.2.3  ???   glp_ios_row_attr
* 5.2.4 Done, glp_ios_mip_gap (tree.c)
* 5.2.5 N/A, glp_ios_node_data (unfortunately GLPK provides no
  	       facilities for determining that the corresponding node has been
	       deallocated -- one would think this would be *absolutely necessary*
               since one may wish to store data of varying sizes for each node
               rather than just a single static block, but heck, what do I know...)
* 5.2.6 Done, glp_ios_select_node (tree.c)
* 5.2.7 Done, glp_ios_heur_sol (tree.c)
* 5.2.8 ???   glp_ios_can_branch
* 5.2.9 ???   glp_ios_branch_upon
* 5.2.10 Done, glp_ios_terminate (tree.c)

## Section 5.3
* 5.3.1  Done, glp_ios_tree_size (tree.c)
* 5.3.2  Done, glp_ios_curr_node (tree.c)
* 5.3.3  Done, glp_ios_next_node (tree.c)
* 5.3.4  Done, glp_ios_prev_node (tree.c)
* 5.3.5  Done, glp_ios_up_node (tree.c)
* 5.3.6  Done, glp_ios_node_level (tree.c)
* 5.3.7  Done, glp_ios_node_bound (tree.c)
* 5.3.8  Done, glp_ios_best_node (tree.c)

# Chapter 6
## Section 6.1
* 6.1.1  N/A, no need to explicitly represent the GLPK long numbers
* 6.1.2  N/A, glp_version (already have glpk.version)
* 6.1.3  N/A, glp_free_env (environment.c)
* 6.1.6  Done, glp_term_out (environment.c)
* 6.1.7  Done, glp_term_hook (environment.c)
* 6.1.8  ??
* 6.1.9  ??
* 6.1.10-6.1.15 N/A, internal routines that don't need to be exposed.
* 6.1.16 Done, glp_mem_usage (environment.c)
* 6.1.17 Done, glp_mem_limit (environment.c)

