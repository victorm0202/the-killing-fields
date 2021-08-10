# Sensitivity analysis of hyperparameters for a Bayesian hierarchical spatio-temporal model with separable space and time effects

Priors distributions considered for precision parameter $\sigma$ in BYM and AR1 models for spatial and temporal effects. Note that all priors in INLA are set in the internal representation of the parameter, therefore, $\sigma=\exp^{-\frac{\theta}{2}}$, and the prior is defined on $\theta$.

- `logGamma1`: LogGamma with parameters shape=1 and rate=.00005
- `logGamma1`: LogGamma with parameters shape=.001 and rate=.001
- `half.Normal`: Half-Normal with zero mean and precision parameter $\tau=.001$ 
- `half.Cauchy`: Half-Cauchy with scale parameter $\gamma=25$
- `half.T`: Half-t with parameter $\nu=3$ degrees of freedom
- `unif`: Uniform improper $p(\sigma)\propto 1$
- `pc.prec`: Penalized complexity prior for precision with parameters $(5, 0.01)$

For details, see ....REFERENCES....

## CAR + AR: full model

### Posterior distribution of fixed effects

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar-Intercept.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar-Crops.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar-Confrontations.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar-Migration route.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar-Trend.png" height="70%" width="70%" align="center"/>

### Spatial random effects. Structured (left) and unstructured (right)

#### logGamma1

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_logGamma1precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_logGamma1precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### logGamma2

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_logGamma2precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_logGamma2precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Normal

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_half.NormalprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_half.NormalprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Cauchy

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_half.CauchyprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_half.CauchyprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.T

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_half.TprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_half.TprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### unif

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_unifprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_unifprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### pc.prec

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_pc.precprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_pc.precprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


### Temporal random effects

<img src="tmpplots_20210805_20/tsplot_temporal_effects_PRIORS_car-Intercept.png" height="70%" width="70%" align="center"/>

## CAR + AR model: Confrontations effect removed

### Posterior distribution of fixed effects

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_enfrentamientos-Intercept.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_enfrentamientos-Crops.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_enfrentamientos-Migration route.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_enfrentamientos-Trend.png" height="70%" width="70%" align="center"/>

### Spatial random effects. Structured (left) and unstructured (right)

#### logGamma1

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_logGamma1precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_logGamma1precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### logGamma2

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_logGamma2precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_logGamma2precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Normal

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_half.NormalprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_half.NormalprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Cauchy

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_half.CauchyprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_half.CauchyprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.T

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_half.TprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_half.TprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### unif

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_unifprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_unifprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### pc.prec

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_pc.precprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_enfrentamientos_pc.precprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


### Temporal random effects

<img src="tmpplots_20210805_20/tsplot_temporal_effects_PRIORS_car_ar_sin_enfrentamientos.png" height="70%" width="70%" align="center"/>

## CAR + AR model: Migration effect removed

### Posterior distribution of fixed effects

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_ruta_migratoria-Intercept.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_ruta_migratoria-Crops.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_ruta_migratoria-Confrontations.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_car_ar_sin_ruta_migratoria-Trend.png" height="70%" width="70%" align="center"/>

### Spatial random effects. Structured (left) and unstructured (right)

#### logGamma1

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_logGamma1precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_logGamma1precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### logGamma2

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_logGamma2precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_logGamma2precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Normal

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_half.NormalprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_half.NormalprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Cauchy

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_half.CauchyprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_half.CauchyprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.T

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_half.TprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_half.TprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### unif

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_unifprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_unifprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### pc.prec

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_pc.precprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_car_ar_sin_ruta_migratoria_pc.precprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


### Temporal random effects

<img src="tmpplots_20210805_20/tsplot_temporal_effects_PRIORS_car_ar_sin_ruta_migratoria.png" height="70%" width="70%" align="center"/>

## ZIP0 + CAR + AR

### Posterior distribution of fixed effects

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip0_car_ar-Intercept.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip0_car_ar-Crops.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip0_car_ar-Confrontations.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip0_car_ar-Migration route.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip0_car_ar-Trend.png" height="70%" width="70%" align="center"/>

### Spatial random effects. Structured (left) and unstructured (right)

#### logGamma1

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_logGamma1precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_logGamma1precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### logGamma2

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_logGamma2precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_logGamma2precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Normal

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_half.NormalprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_half.NormalprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Cauchy

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_half.CauchyprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_half.CauchyprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.T

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_half.TprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_half.TprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### unif

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_unifprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_unifprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### pc.prec

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_pc.precprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip0_car_ar_pc.precprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


### Temporal random effects

<img src="tmpplots_20210805_20/tsplot_temporal_effects_PRIORS_zip0_car_ar.png" height="70%" width="70%" align="center"/>

## ZIP1 + CAR + AR

### Posterior distribution of fixed effects

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip1_car_ar-Intercept.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip1_car_ar-Crops.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip1_car_ar-Confrontations.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip1_car_ar-Migration route.png" height="70%" width="70%" align="center"/>

<img src="tmpplots_20210805_20/dist_post_fix_effects_PRIORS_zip1_car_ar-Trend.png" height="70%" width="70%" align="center"/>

### Spatial random effects. Structured (left) and unstructured (right)

#### logGamma1

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_logGamma1precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_logGamma1precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### logGamma2

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_logGamma2precSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_logGamma2precUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Normal

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_half.NormalprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_half.NormalprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.Cauchy

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_half.CauchyprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_half.CauchyprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### half.T

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_half.TprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_half.TprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### unif

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_unifprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_unifprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


#### pc.prec

<table align='center'>
<tr>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_pc.precprecSpatial_.png" height="90%" width="90%"/></td>
<td><img src="tmpplots_20210805_20/spplot_spatial_effects_zip1_car_ar_pc.precprecUnstruct_.png" height="90%" width="90%"/></td>
</tr>
</table>


### Temporal random effects

<img src="tmpplots_20210805_20/tsplot_temporal_effects_PRIORS_zip1_car_ar.png" height="70%" width="70%" align="center"/>
