
#. reset (IO devices are reset)
#. setup kernel memory management

    #. first 6 pages map to identical address in PA
    #. 7th page map to user blocks segment which is at first block boundary after kernel code
    #. 8th page map to IO registers

#. clear bss
#. clear user blocks
#. call main
#. return to user space
