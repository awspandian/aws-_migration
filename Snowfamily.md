AWS Snowball and Snowmobile are used for migrating large volumes of data to AWS
Snowball Edge Compute Optimized
	Provides block and object storage and optional GPU • Use for data collection, machine learning and processing, and storage in environments with intermittent connectivity (edge use cases)
Snowball Edge Storage Optimized
	Provides block storage and Amazon S3-compatible object storage
	Use for local storage and large-scale data transfer  
Snowcone
	Small device used for edge computing, storage and data transfer
	Can transfer data offline or online with AWS DataSync agent
	
 Uses a secure storage device for physical transportation
 Snowball Client is software that is installed on a local computer and is used to identify, compress, encrypt, and transfer data
 Uses 256-bit encryption (managed with the AWS KMS) and tamper-resistant enclosures with TPM
 Snowball (80TB) (50TB ) “petabyte scale”
 Snowball Edge (100TB) “petabyte scale”
 Snowmobile – “exabyte scale” with up to 100PB per Snowmobile
 
 Ways to optimize the performance of Snowball transfers:
1. Use the latest Mac or Linux Snowball client
2. Batch small files together
3. Perform multiple copy operations at one time
4. Copy from multiple workstations
5. Transfer directories, not files

Snowball Use Cases
	• Cloud data migration – migrate data to the cloud
	• Content distribution – send data to clients or customers
	• Tactical Edge Computing – collect data and compute
	• Machine learning – run ML directly on the device
	• Manufacturing – data collection and analysis in the factory
	• Remote locations with simple data–pre-processing, tagging, compression etc.
