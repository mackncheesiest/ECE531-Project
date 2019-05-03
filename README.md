# ECE531-Project: FSK
Authors: Joshua Mack & Ezra Muir

## Overview
This repository contains GNU Radio Flowgraphs associated with FSK modulation and demodulation as well as sample FSK-based keyfob data files that can be used in lieu of an actual keyfob.

* FSK_RX_Flowgraph.grc: a flowgraph that presents basic ability to receive 2-FSK signals using the quadrature demodulator block

* FSK_TX_Flowgraph.grc: a flowgraph that presents basic ability to transmit a 2-FSK synthetic signal

* RX_TX_To-From_File.grc: a flowgraph that simply gives the user the ability to enable one part of the graph and receive+write to a file or enable another part of the graph and read+transmit that file with a common set of sample rate, rf bandwidth, etc parameters shared between the two. This helps avoid issues with two flowgraphs becoming out of sync with different parameter values.

* data_files: a set of captured FSK keyfob signals at a variety of sample rates 

## Usage

Each flowgraph is a self contained unit that can simply be run in GNU Radio Companion. 

If using a file source in the FSK_RX_Flowgraph, care may need to be taken to ensure that the proper file is selected and that it isn't using an absolute path that doesn't exist on your machine. 
