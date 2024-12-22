# Go Map Access Panic

This repository demonstrates a common but easily overlooked error in Go: accessing a map element when the map is nil.  This operation will cause a panic.

## The Bug

The `bug.go` file contains code that attempts to access a map element without first checking if the map is initialized.  This leads to a runtime panic.

## The Solution

The `bugSolution.go` file provides a corrected version, demonstrating safe map access using the `if` statement to check for a nil map.