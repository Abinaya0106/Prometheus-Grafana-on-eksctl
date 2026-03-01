# Metrics Server Troubleshooting

## Issue

kubectl top nodes Error: Metrics API not available

## Root Cause

APIService was not fully registered.

## Fix

Edit deployment and add: --kubelet-insecure-tls

kubectl edit deployment metrics-server -n kube-system

## Verification

kubectl get deployment metrics-server -n kube-system
