my repo

Hello World!

require 'nngraph'
require 'fast_neural_style.NoiseFill'

function defineG_encoder_decoder(input_nc, output_nc, ngf)
    local netG = nil
    -- input is (nc) x 256 x 256
    local e1 = -nn.SpatialConvolution(input_nc, ngf, 4, 4, 2, 2, 1, 1)
