# Implementation-of-3D-Vascular-Network-Formation-Confined-in-a-Defined-Geometry

# 3D Vascular Network Simulation in Liver Lobule Geometry

## Overview
A Python-based computational framework simulating 
3D vascular network formation within a liver lobule 
geometry using space colonization algorithms driven 
by physiologically-motivated VEGF and oxygen gradients.

## Biological Background
The liver lobule is the functional unit of the liver, 
structured as a hexagonal prism (~1.5mm diameter, 1mm 
height) with:
- **Central vein** at the geometric center — low oxygen, 
  high VEGF expression
- **Portal triads** at 6 hexagonal vertices — high oxygen, 
  blood entry points
- **Oxygen gradient** decreasing from portal triads 
  toward central vein
- **VEGF gradient** increasing toward central vein, 
  driving angiogenesis into hypoxic regions

## Computational Approach
- **Geometry:** Hexagonal prism modeled in Autodesk 
  Fusion 360, exported as STL and imported into Python
- **Vascular growth:** Space colonization algorithm — 
  vessels grow from portal triads toward VEGF-weighted 
  attraction points
- **VEGF model:** Exponential decay from central vein 
  simulating diffusion-based gradient
- **Oxygen model:** Linear gradient from portal triads 
  to central vein based on Rappaport acinar zones
- **Geometric constraint:** Vessel growth confined 
  within hexagonal boundary

## Repository Structure
