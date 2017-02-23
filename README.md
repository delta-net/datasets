# Delta-net

Delta-net is tool that makes it possible to detect and prevent certain network
outages before they occur. For this, Delta-net analyzes changes to the data plane
in real-time and incrementally maintains flow information of every packet in the
entire network. In our NSDI'17 paper, we propose the first provably quasi-linear
algorithm to do so. Here, we provide the data sets that we used in our experiments.

If you are interested to learn more, please check out [our publications](#publications).
For any questions, feel also free to contact us.

## Data Sets

Our [NSDI'17 data set][data-set-nsdi-17] comprise several hundred million IP prefix
rules generated using topologies and BGP updates from real-world deployed networks,
including a globally deployed [ONOS][onos] software-defined networking application,
called [SDN-IP][sdn-ip].

Our experiments show that Delta-net checks a rule insertion and removal in tens of
microseconds on average, a more than 10X improvement over the state-of-the-art. We
also show that Delta-net eliminates an inherent bottleneck in the state-of-the-art
that restricts its use in answering Datalog-style "what if" queries.

[sdn-ip]: https://wiki.onosproject.org/display/ONOS/SDN-IP+Architecture
[onos]: http://onosproject.org/
[data-set-nsdi-17]: https://mega.nz/#!WgYBSZqC!pruWLWKse4KA60Mb35p4CE2eaJ-d1zyX4PkaO2PNWA0

## Publications

```
@inproceedings{HKP2017,
 author = {Horn, Alex and Kheradmand, Ali and Prasad, Mukul R.},
 title = {Delta-net: Real-time Network Verification Using Atoms},
 booktitle = {NSDI},
 year = {2017},
}
```

## Notice

```
THIS DATASET IS PROVIDED "AS IS" BY THE PREPARER OF THE DATA SET. BY USING THE
DATASET, YOU EXPRESSLY UNDERSTAND AND AGREE THAT, EXCEPT TO THE EXTENT
PROHIBITED BY LAW, ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
PURPOSE OR SPECIFIC PERFORMANCE USING SUCH DATASET AND/OR ANY WARRANTIES THAT
THIS DATASET WILL BE ERROR FREE OR FREE OF HARMFUL COMPONENTS, ARE DISCLAIMED.
IN NO EVENT SHALL THE COPYRIGHT HOLDER OR PREPARER OF  DATASET OR ITS COMPANY
OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
IN ANY WAY OUT OF THE USE OF THIS DATASET EVEN IF ADVISED OF THE POSSIBILITY OF
SUCH DAMAGE.

You understand and agree that you will not: 1) make false or misleading
statements or representations regarding Fujitsu or Fujitsu products and
services; 2) take on any obligation or responsibility, or make any
representation, warranty, guarantee or endorsement to anyone on Fujitsu's behalf
(including, without limitation, any of our products or services); and that you
will not state or imply that Fujitsu has developed, endorsed, reviewed or
otherwise approved of any of your products particularly through the use of this
DATASET. You agree that you will indemnify, defend and hold us harmless from
and against any and all claims which may arise under or out of your use of the
DATASET whether lawful or unlawful and you shall not be in violation of any of
the terms of service or other terms of the github.com website or any other website
where the DATASET is posted; your negligence or intentional misconduct; your
products, or any integrations you develop, design, promote or distribute using
the Software; any misrepresentations you make with respect to Fujitsu, or
Fujitsu products or services.
```
