CANUCS_double_break_candidates.dat
Desprez et al. (2024)
README last modified: Mar. 14th 2024


Notes
----------------------------------------

1) List of available bands
List of HST/ACS bands:        F435W, F606W, F814W
List of HST/WFC3/UVIS bands:  F438WU, F606WU
List of HST/WFC3/IR bands:    F105W, F125W, F140W, F160W
List of JWST/NIRCam bands:    F090W, F115W, F140M, F150W, F162M, F182M, F200W, F210M, F250M, F277W, F300M, F335M, F356W, F360M, F410M, F444W

2) Fluxes and flux errors
Fluxes are derived through corrected 0.3" aperture photometry corrected to total (Kron) on the F444W band.
f_tot{BAND} = f_aper{BAND} * (f_tot{F444W} / f_aper{F444W})
Errors are estimated from empty apertures in noise-normalized images background.

3) Missing data
Missing data are marked by:   -99.0


Columns       Units         Description
----------------------------------------
ID:                         Source ID
RA:           [deg]         Right ascension
DEC:          [deg]         Declination
{BAND}:       [nJy]         Total flux in nJy
{BAND}e:      [nJy]         Flux error in nJy
z50_phos:                   Median photometric redshift, Phosphoros fit
z16_phos:                   16th percentile photometric redshift, Phosphoros fit
z84_phos:                   84th percentile photometric redshift, Phosphoros fit
zb_phos:                    Best fit photometric redshift, Phosphoros fit
zb_eazy:                    Best fit photometric redshfit, EAzY fit
zspec:                      NIRSpec prism redshift
zspec_e:                    NIRSpec prism redshift fit error
mu50:                       Median value of strong lensing magnification (assuming zspec or Phosphoros redshift PDF)
mu16:                       16th percentile of strong lensing magnification (assuming zspec or Phosphoros redshift PDF)
mu84:                       84th percentile of strong lensing magnification (assuming zspec or Phosphoros redshift PDF)
mass50_DB:    [log(Msun)]   Median log of stellar mass, fit from Dense Basis, magnification corrected
mass16_DB:    [log(Msun)]   16th percentile log of stellar mass, fit from Dense Basis, magnification corrected
mass84_DB:    [log(Msun)]   84th percentile log of stellar mass, fit from Dense Basis, magnification corrected
mass50_BP:    [log(Msun)]   Median log of stellar mass, fit from Bagpipes, magnification corrected
mass16_BP:    [log(Msun)]   16th percentile log of stellar mass, fit from Bagpipes, magnification corrected
mass84_BP:    [log(Msun)]   84th percentile log of stellar mass, fit from Bagpipes, magnification corrected
